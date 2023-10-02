# Desafio Back-end SCS

Primeiramente, parabéns por chegar nessa etapa do processo seletivo, estamos muito felizes
Abaixo você encontrará todos as informações necessárias para iniciar o seu teste.

## Avisos antes de começar

- Crie um repositório no seu GitHub **sem citar nada relacionado a SCS**.
- Faça seus commits no seu repositório.
- Envie o link do seu repositório para o email **tracy@tracy.com**.
- Você poderá consultar o Google, Stackoverflow ou algum projeto particular na sua máquina.
- Dê uma olhada em como será a [entrevista](#para-o-dia-da-entrevista-técnica).
- Fique à vontade para perguntar qualquer dúvida aos recrutadores.
- Fique tranquilo, respire, assim como você, também já passamos por essa etapa. Boa sorte! :)

*Corpo do Email com o link do repositório do desafio*

>Seu Nome
>
>
>Link do repositório
>
>Link do Linkedin

### Sobre o ambiente da aplicação:

- Escolha qualquer a linguagem ou framework que se sinta **confortável** em trabalhar. Esse teste **não faz** nenhuma preferência, portanto decida por aquele com o qual estará mais seguro em apresentar e conversar com a gente na entrevista ;)

- Você pode, inclusive, não optar por framework nenhum.

- Ainda assim, se optar por um framework tente evitar usar muito métodos mágicos ou atalhos já prontos. Sabemos que essas facilidades aumentam a produtividade no dia-a-dia mas aqui queremos ver o **seu** código e a sua forma de resolver problemas.

- Valorizamos uma boa estrutura criada por você.

## Para o dia da entrevista técnica
Na data marcada compareça no local com sua aplicação funcionando na sua máquina, caso não tenha como fazer isso, sinalize no e-mail que você não poderá levar o ambiente para demonstração, assim os recrutadores poderam executar nas suas próprias máquinas. Prepare-se pra uma revisão junto com a gente da sua solução :). Você poderá explicar o que pensou ao desenvolver e como podemos evoluir ou melhorar o projeto.

## Objetivo: Cadastro de produtos

Temos uma plataforma onde os usuários podem cadastrar, atualizar, visualizar e deletar produtos. Cada produto tem um nome, descrição, preço e quantidade em estoque.

Requisitos:

- O nome do produto é obrigatório e deve ser único no sistema. Seu sistema deve permitir apenas um cadastro com o mesmo nome de produto.

- A descrição do produto é opcional, mas se fornecida, deve ter no máximo 500 caracteres.

- O preço do produto deve ser um valor positivo e é obrigatório.

- A quantidade em estoque do produto deve ser um valor inteiro positivo e é obrigatório.

- O sistema deve permitir a atualização de qualquer um dos campos do produto, respeitando as validações acima.

- O sistema deve permitir a visualização de um produto específico, bem como a listagem de todos os produtos cadastrados.

- O sistema deve permitir a exclusão de um produto.

- Este serviço deve ser RESTFul.

### Payload

Aqui está uma proposta de payload para o CRUD de produtos:

POST /products

```json
{
    "name": "Nome do Produto",
    "description": "Descrição do Produto",
    "price": 100.00,
    "stock": 10
}
```

PUT /products/{productId}

```json
{
    "name": "Nome do Produto Atualizado",
    "description": "Descrição do Produto Atualizada",
    "price": 150.00,
    "stock": 15
}
```

GET /products/{productId}

```json
{
    "id": 1,
    "name": "Nome do Produto",
    "description": "Descrição do Produto",
    "price": 100.00,
    "stock": 10
}
```

GET /products

```json
[
    {
        "id": 1,
        "name": "Nome do Produto",
        "description": "Descrição do Produto",
        "price": 100.00,
        "stock": 10
    },
    ...
]
```

# Avaliação

Apresente sua solução utilizando o framework que você desejar, justificando a escolha.
Atente-se a cumprir a maioria dos requisitos, pois você pode cumprir-los parcialmente e durante a avaliação vamos bater um papo a respeito do que faltou.

Teremos 2 partes da avaliação:

A correção objetiva será realizada através da utilização de um script de correção automatizada. **ATENTE-SE AOS CONTRATOS E URLS NOS REQUISITOS**



A correção qualitativa será durante a entrevista e levará em conta os seguintes critérios:

## O que será avaliado e valorizamos :heart:
- Código limpo e organizado (nomenclatura, etc)
- Ser consistente e saber argumentar suas escolhas
- Apresentar soluções que domina
- Modelagem de Dados
- Manutenibilidade do Código
- Tratamento de erros
- Cuidado com itens de segurança
- Carinho em desacoplar componentes

De acordo com os critérios acima, iremos avaliar seu teste para avançarmos para a entrevista técnica.


## O que será um Diferencial
- Uso de Docker
- Testes de [integração](https://www.atlassian.com/continuous-delivery/software-testing/types-of-software-testing)
- Testes [unitários](https://www.atlassian.com/continuous-delivery/software-testing/types-of-software-testing)
- Uso de Design Patterns
- Documentação
- Proposta de melhoria na arquitetura


## Dividas entre em contato

geovanefeitosacavalcante@gmail.com,
vfranca477@gmail.com,
hugo.bandeira@hotmail.com

