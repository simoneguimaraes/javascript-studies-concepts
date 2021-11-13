# Conceitos do JavaScript

## Conceitos Básicos
- if, for, lógica
- Como manipular o DOM? Colocou um dado no input, como você usa esse valor no JS.
- Se clicou em um botão, como voce manipula o evento click.
- Como manipular arrays

## Como fazer sites institucionais estáticos
- Entender a semântica das tags

## JavaScript
- Formulários
- Const var let
- Hoisting
- Array - filter, map, reduce
- Funcão normal x arrow function
- Requisições com Axios - APIs públicas *Youtube: agência de viagens e Dashboard do Star Wars usando API pública

## Como fazer uma lista de tarefas
- Criar um campo de input para adicionar elementos
- Adiciona elementos no array
- Deleta itens do array
- Reordenar o array
- Como marcar quais tarefas voce ja fez

## JS é uma linguagem orientada a objetos

- O JS é um sistema de tipos - tipos primitivos e complexos
- O JS nao é fortemente tipada - podemos declarar uma variável sem especificar o tipo de valor. E o tipo pode mudar.

```Existem os dados de tipo primitivo (number, string, boolean, undefined, null, symbol). O restante é Objeto (Arrays, funções, objetos, regex).```

```O que muda entre esses tipos de dados é que **os dados de tipo primitivo são declarados como valor** e **os objetos são passados como referência**.```
## Imutabilidade nos Tipos de Dados

- A mutabilidade e a imutabilidade estão relacionados ao fato de que, quando você copia o dado, ele altera ou não o seu original.
- Quando você faz uma cópia de dados primitivos, o original nunca muda.
- Quando você faz uma cópia de dados do tipo objeto, o original é alterado.

### Dados do tipo primitivo
Os dados de **tipo primitivo** são passados por **valor** e são **imutáveis**:
```
let name = 'Carlos'
let firstName = name
```

- Quando voce cria as duas variáveis de tipo primitivo, é criado um ponto de memória específico pra ele.
- Então se eu alterar name, firstName não é alterado. 
Se eu fizer:
```
let fullName = 'Simone Guimaraes'
let firstName = fullName.slice(0, 6)
console.log(firstName) // 'Simone'
```
A variável fullName não será alterada.

### Dados do tipo Objeto
Os dados que são do **tipo Objeto** são passados por **referência** e são **mutáveis**:
```
let name = {}
let firstName = name
```

- Quando voce cria a variável de tipo objeto 'name', é criado um ponto de memória específico pra ele. Porém, quando voce cria a variável 'firstName' que tem como referência o 'name', não é criado outro espaço de memória para ele. 
- Os dois vão apontar para *o mesmo espaço na memória*.
- Então se eu alterar name, firstName é alterado e vice-versa. 
Se eu fizer:
```
let numbers = [4, 3, 2, 1]
let orderedNumbers = numbers.sort()
console.log(numbers) // [1, 2, 3, 4]
```
A variável numbers foi alterada, sofreu uma mutação.


## Tópicos
Como usar as tags HTML certas
CSS rápido - reaproveitamento de classes, usar flexbox, fazer responsividade
Saber os principais métodos - map, filter, reduce
Diferença entre as variáveis const, let e var
O que é Hoisting, Escopo, Arrow Function
O que significa Linguagem Orientada a Objetos
https://github.com/isadorastan/estudos

### Hoisting

- JavaScript's interpreter appears to move the declaration of functions, variables or classes to the top of their scope, prior to execution of the code.
- One of the advantages of hoisting is that it **lets you use a function before you declare it in your code**. 
- Hoisting works with variables too, so you can use a variable in code before it is declared and/or initialized. 
- However JavaScript only hoists declarations, not initializations! This means that initialization doesn't happen until the associated line of code is executed, even if the variable was originally initialized then declared, or declared and initialized in the same line.

### Scope


### Arrow Function
Difference between an arrow function and a normal function
