<h1>Workshop MySQL</h1>

> Status: Completo ✔️

### Backend de uma aplicação de loja, projetado para fornecer uma API RESTful

## Funcionalidade Principal:

+ Gerenciamento de Usuários: Adicionar, recuperar, deletar e atualizar usuários. Com associação direta com outras classes como pedidos, produtos e categorias.

## A aplicação fornece os seguintes endpoints da API RESTful:

### Usuários:

- **GET /api/users**: Retorna todos os usuários cadastrados.
- **GET /api/users/{id}**: Retorna um usuário específico com o ID fornecido.
- **POST /api/users**: Cria um novo usuário com os dados fornecidos no corpo da requisição.
- **PUT /api/users/{id}**: Atualiza os dados de um usuário existente, exceto a senha, com o ID fornecido.
- **DELETE /api/users/{id}**: Remove um usuário existente com o ID fornecido.

#### Exemplo de corpo de requisição para criar um usuário:

```json
{
  "name": "Fulano Silva",
  "email": "fulano@gmail.com",
  "phone": "918288488",
  "password": "senha123"
}
```

#### Exemplo de corpo de requisição para atualizar um usuário:

```json
{
  "name": "Fulano Rodrigues",
  "email": "fulano@hotmail.com",
  "phone": "390288488",
}
```

### Pedidos:

- **GET /api/orders**: Retorna todos os pedidos registrados.
- **GET /api/orders/{id}**: Retorna um pedido específico com o ID fornecido.

### Produtos:

- **GET /api/products**: Retorna todos os produtos registrados.
- **GET /api/products/{id}**: Retorna um produto específico com o ID fornecido.

### Categorias:

- **GET /api/categories**: Retorna todos as categorias registradas.
- **GET /api/categories/{id}**: Retorna uma categoria específica com o ID fornecido.

## Campos do modelo do Usuário:

+ id
+ name
+ email
+ phone
+ password

## Campos do modelo do Pedido:
+ id
+ moment
+ orderStatus
+ client
+ items
+ payment
+ total

## Campos do modelo do Produto:
+ id
+ name
+ description
+ price
+ imgUrl
+ categories

## Campos do modelo da Categoria:
+ id
+ name

## Tecnologias Usadas:

<table>
  <tr>
    <td>Java</td>
    <td>Spring Boot</td>
    <td> MySQL</td>
  </tr>
  <tr>
    <td>17.0</td>
    <td>3.1.1</td>
    <td>8.0</td>
  </tr>
</table>

## Como executar o Projeto:

```bash
# clonar repositório
1) git clone git@github.com:Gustasszz/workshop.git

# entrar na pasta do projeto workshop
2) cd workshop

# executar o projeto
3) ./mvnw spring-boot:run
```
