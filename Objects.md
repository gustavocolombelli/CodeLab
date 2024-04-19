## Exercícios de Objects

#### Exercício 1 - Básico de objetos
1.1 Crie um objeto chamado pessoa que represente uma pessoa com as propriedades nome, idade e profissao.

1.2 Atribua valores nas propriedades nome, idade e profissão 

1.3 Imprima apenas o valor da propriedade nome do objeto

1.4 Sobrescreva o valor da propriedade nome do objeto

1.5 Adicione uma nova propriedade chamada cidade, e atribua um valor a esta propriedade

1.5 Delete a propriedade profissão

1.6 Imprima o objeto por completo

<details>
<summary>Resposta</summary>

```javascript
let pessoa = {
  nome: "Gustavo",
  idade: 29,
  profissao: "Dev"
}

console.log(pessoa.nome);

pessoa.nome = "Josimar"

pessoa.cidade = "Recife"

delete pessoa.profissao;

console.log(pessoa);

```
</details>

### Exercício 2

Neste exercício prático, seu objetivo é criar um objeto que represente um produto para ser exibido em um card de uma loja online. 
O objeto deve conter informações essenciais sobre o produto, incluindo nome, preço, descrição, imagem, disponibilidade, avaliação, características e tags.

2.1 Estrutura do dado

| Propriedade    | Tipo de Dado | Exemplo                                                                        |
|----------------|--------------|--------------------------------------------------------------------------------|
| Nome           | Textual       | "Smartphone XYZ"                                                              |
| Preço          | Numérico       | 999.99                                                                         |
| Descrição      | Textual       | "Um smartphone poderoso com câmera de alta resolução e processador rápido."  |
| Imagem         | Textual       | "caminho/para/imagem.jpg"                                                     |
| Disponível     | Booleano      | true                                                                           |
| Avaliação      | Numérico       | 4.5                                                                            |
| Características| Array de Textos       | ["Tela de 6 polegadas", "Memória interna de 128GB", "Câmera principal de 48MP"] |
| Tags           | Array de Textos       | ["tecnologia", "smartphone", "eletrônicos"]                                    |

2.2 Crie duas funções como propriedade deste objeto, estas funções serão responsável por imprimir as características e tags do produto

2.3 Crie 4 objetos com características diferentes porém respeitando a estrutura de dado de 2.1

2.4 Inicialize uma variável do tipo array chamado listaDeProdutos, e adicione no array os 4 objetos criados.

2.5 Imprima todos os produtos que você criou.



