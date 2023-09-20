# Typescript
## Tipagem
 - A tipagem é feita automaticamente quando possivel.
 - Quando a tipagem de alguma coisa não fica clara é possivel declarar a tipagem assim:
   ```
   const stringTeste: string = "Olá"
   ```
 - As vezes é inviavel declarar um tipo como por exemplo no evento "onclick", então o tipo any é usado. Ex:
    ```
     onClick: any => void;
## Interface
  - Quando um algo recebe uma coisa com varias propriedades, como por exemplo um objeto é nescessario fazer uma interface. Ex:
    ```
    interface ButtonProps {
    symbol: string;
    style: string;
    }
   E para aplicar:
   ```
  const Button = (props: ButtonProps) => {}
  ```
  - Quando você quiser que uma tipagem seja opcional, use "?" após o nome da variavel. Ex:
    ```
    interface ButtonProps {
    symbol?: string;
    style?: string;
    }
  - "Props" é usada para passar interfaces, é possivel usar interfaces de outros arquivos com ela.
  - https://www.typescriptlang.org/docs/handbook/2/basic-types.html
## Modulos
  - É nescessário declarar tipos de arquivo baseado na extensão quando usar import fazendo um arquivo de modulo. Ex: svg.d.ts
    ```
    declare module '*.svg' {
    const content: any;
    export default content;
    }
  
