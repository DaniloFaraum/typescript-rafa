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
- omitir com ?
## Interface
  -Quando um algo recebe uma coisa com varias propriedades, como por exemplo um objeto é nescessario fazer uma interface. Ex:
  
    interface ButtonProps {
    symbol: string;
    style: string;
    }
  - como aplicar interface
  - https://www.typescriptlang.org/docs/handbook/2/basic-types.html
