> [!NOTE]
>Imprimir com o console é uma maneira de exibir informações, mensagens de erro, variáveis e resultados de código no console do navegador ou
>no console de desenvolvedor do ambiente de desenvolvimento. Isso é útil para depurar, testar comportamento de variáveis, diagnosticar problemas e avaliar o comportamento do código durante o desenvolvimento

```javascript
console.log();
console.error();
console.warn();
console.info()
```
### Exercícios e fixação

#### 1. Utilizando as funções de impressão, implemente os exercícios a seguir:
* 1.1\. Imprima "Olá mundo"
* 1.2\. Imprima "Ocorreu um erro inesperado!" utilizando a função correspondente
* 1.3\. Imprima "Essa é uma mensagem informativa!" utilizando a função correspondente
* 1.4\. Imprima "Esse é um aviso que requer atenção!" utilizando a função correspondente
* 1.5\. Imprima no console o número 5
* 1.6\. Imprima no console o número 6 dividido por 3
* 1.7\. Imprima no console o número 10 multiplicado por 10
* 1.8\. Imprima no console o número 10 dividido por 0
* 1.9\. Imprima no console o valor booleano true

<details>
<summary>Respostas</summary>

```javascript
    console.log("Olá mundo!");
    //Output: Olá mundo!

    console.error("Ocorreu um erro inesperado!");
    //Output: Ocorreu um erro inesperado!
    
    console.error("Essa é uma mensagem informativa!");
    //Output: Essa é uma mensagem informativa!

    console.error("Esse é um aviso que requer atenção!");
    //Output: Esse é um aviso que requer atenção!

    console.log(5);
    //Output: 5

    console.log(6/3);
    //Output: 2

    console.log(10*10);
    //Output: 100

    console.log(10/0);
    //Output: Infinity

    console.log(true);
    //Output: true
```
</details>

#### 2. Utilizando o operador `typeof` para imprimir os tipos dos exercícios a seguir
* 2.1\. Imprima o tipo de dado de: "Ola mundo"
* 2.2\. Imprima o tipo de dado de: 5
* 2.3\. Imprima o tipo de dado de: 12.4
* 2.4\. Imprima o tipo de dado de: true
* 2.5\. Imprima o tipo de dado de: false
* 2.6\. Imprima o tipo de dado de: 50/0
* 2.7\. Imprima o tipo de dado de: 20410241024n
<details>
<summary>Respostas</summary>

```javascript

console.log(typeof "Olá mundo");

console.log(typeof 5);

console.log(typeof 12.4)

console.log(typeof true)

console.log(typeof false)

console.log(typeof 50/0)

console.log(typeof 120410241024n)

```
</details>


