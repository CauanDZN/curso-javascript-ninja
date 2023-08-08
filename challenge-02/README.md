# Desafio da semana #2

Nesse exercício, você está livre para escolher os nomes para suas variáveis e funções! :smile:

```js
// Crie uma função que receba dois argumentos e retorne a soma dos mesmos.
function soma(a, b){
    let soma = a + b;
    return soma;
}

// Declare uma variável que receba a invocação da função criada acima, passando dois números quaisquer por argumento, e somando `5` ao resultado retornado da função.
let somatorio = soma(5, 5) + 5

// Qual o valor atualizado dessa variável?
15

// Declare uma nova variável, sem valor.
let variavelsemvalor

/*
Crie uma função que adicione um valor à variável criada acima, e retorne a string:
    O valor da variável agora é VALOR.
Onde VALOR é o novo valor da variável.
*/
function novoValor(variavel){
  variavel = "CAUAN"
  return "O valor da variável agora é " + variavel
}

// Invoque a função criada acima.
console.log(novoValor(variavelsemvalor))

// Qual o retorno da função? (Use comentários de bloco).
"O valor da variável agora é CAUAN"

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos;
2. Se qualquer um dos três argumentos não estiverem preenchidos, a função deve retornar a string:
    Preencha todos os valores corretamente!
3. O retorno da função deve ser a multiplicação dos 3 argumentos, somando `2` ao resultado da multiplicação.
*/
function multiplicacao(a, b, c){
  if (a && b && c){
    multi = a * b * c;
    soma = multi + 5;
    return soma;
  } else {
    return "Preencha todos os valores corretamente!";
  }
}

// Invoque a função criada acima, passando só dois números como argumento.
console.log(multiplicacao(2, 4))

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
"Preencha todos os valores corretamente!"

// Agora invoque novamente a função criada acima, mas passando todos os três argumentos necessários.
console.log(multiplicacao(2, 4, 5))

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
45

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos.
2. Se somente um argumento for passado, retorne o valor do argumento.
3. Se dois argumentos forem passados, retorne a soma dos dois argumentos.
4. Se todos os argumentos forem passados, retorne a soma do primeiro com o segundo, e o resultado, dividido pelo terceiro.
5. Se nenhum argumento for passado, retorne o valor booleano `false`.
6. E ainda, se nenhuma das condições acima forem atendidas, retorne `null`.
*/
function parametros(a, b, c){
  if(a && !b && !c){
    return a
  }
  else if(a && b && !c){
    let soma = a + b
    return soma
  }
  else if (a && b && c){
    let soma = a + b
    let resultado = soma / c
    return resultado
  }
  else if (!a && !b && !c){
    return false
  }
  else {
    return null
  }
}

// Invoque a função acima utilizando todas as possibilidades (com nenhum argumento, com um, com dois e com três.) Coloque um comentário de linha ao lado da função com o resultado de cada invocação.
console.log(parametros())
console.log(parametros(5))
console.log(parametros(5, 5))
console.log(parametros(5, 5, 2))
```