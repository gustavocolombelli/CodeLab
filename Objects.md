## Exercícios de Objects

#### Exercício 1 - Manipulando objetos

* 1.1\. Crie um objeto chamado pessoa que represente uma pessoa com as propriedades nome, idade e profissao.
* 1.2\. Atribua valores nas propriedades nome, idade e profissão 
* 1.3\. Imprima apenas o valor da propriedade nome do objeto
* 1.4\. Sobrescreva o valor da propriedade nome do objeto
* 1.5\. Adicione uma nova propriedade chamada cidade, e atribua um valor a esta propriedade
* 1.6\. Delete a propriedade profissão
* 1.7\. Imprima o objeto por completo

<details>
<summary>Sugestão de Resposta</summary>

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

* 2.1\. Analise a Estrutura do dados a seguir

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

* 2.2\. Crie duas funções como propriedade deste objeto, estas funções serão responsável por imprimir as características e tags do produto

* 2.3\. Crie 4 objetos com características diferentes porém respeitando a estrutura de dado de 2.1

* 2.4\. Inicialize uma variável do tipo array chamado listaDeProdutos, e adicione no array os 4 objetos criados.

* 2.5\. Imprima todos os produtos que você criou.

* 2.6\.

*2.7\.  Utilizando as funções javascript de manipulação de DOM, realize a implementação de uma funçao que realizará a formação da apresentação do html e informações de um produto essa função, inicialmente irá injetar 1 card no html contendo as informações do produto
<details>
<summary>Sugestão de Resposta</summary>

```javascript
function Produto(nome, preco,
                descricao, imagem, 
                disponivel, avaliacao,
                caracteristicas, tags, porcentagemDesconto
                )
{
    this.nome = nome;
    this.preco = preco;
    this.descricao = descricao
    this.imagem = imagem;
    this.disponivel = disponivel;
    this.avaliacao = avaliacao
    this.caracteristicas = caracteristicas
    this.tags = tags;
    this.porcentagemDesconto = porcentagemDesconto;

    this.imprimeTags = function(){
        this.tags.forEach((currentTag)=>{ //arrow function
            console.log(currentTag);
        })
    };   

    this.imprimeCaracteristicas = function(){
        console.log(this.caracteristicas.join(", "));
    };

    this.getPrecoDesconto = function(){
        return this.preco * (this.porcentagemDesconto==0?1:this.porcentagemDesconto/100)
    }

    this.getPrecoFinal = function(){
        return  this.preco - this.getPrecoDesconto()
    };

    this.imprimePrecoComDesconto = function(){
        console.log(`R$ ${this.getPrecoFinal()} ${this.porcentagemDesconto==0?"":"(Desconto de " + this.porcentagemDesconto + "%)"}`)

        verdadeiro?verdadeiro:false
    };
}

let produto1 = new Produto("xiamomi", 1000, "cel 15 polegadas",
"/caminho/imagem,", true, 5, ["15 polegadas", "android 5.3"], ["celular", "xiaomi"], 2)

produto1.imprimePreco()

```
</details>

