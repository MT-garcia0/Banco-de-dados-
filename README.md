# Banco de dados
_É uma forma estruturada de uma forma de armazenar informações fazendo que seja facilmente acessadas gerenciadas e atualizadas podendo conter todo tipo de dados como números textos imagens entre outros_

## Tipos de Banco de dados
 - _Bancos de dados relacionais_
- _Bancos de dados não relacionais_

## Banco de dados Relacional:
_Um banco de dados relacional é um banco de dados que armazena e fornece acesso relacionados entre si sendo um modelo relacional de uma maneira direta representando dados em tabelas com cada linha na tabela é um registro com uma ID chamada chave_ 

### Exemplo:
_Um exemplo simples séria uma tabela sobe o gerencia mento de uma livraria com as informações do cilente como o nome e o email da pessoa já na segunda tabela seria sobre o livro como o título o autor e o preço do produto_.

## Banco de dados não relacional:
_É um tipo de sistema diferente pois em vez de usar tabelas ele usa um modelo mais flexível como documentos colunas ou graficos para armazenar e acesar informações_.

## O que é normalização e objetivo:
_É um proceso para organizar os dados de forma eficiente a redundância e melhorando a integridade dos dados isso sendo feito através da aplicação de regras que visam evitar anomalis de dados_.

## Exemplo de Tabela não normalizada


| Pedido_ID | Cliente_Nome  | Cliente_Endereço | Produto_ID | Produto_Nome | Quantidade | Preço_Unitário |
|-----------|---------------|------------------|------------|--------------|------------|----------------|
| 1         | João Silva    | Rua A, 123       | 10         | Caneta       | 2          | 4,00           |
| 1         | João Silva    | Rua A, 123       | 11         | Lápis        | 1          | 2,00           |
| 2         | Maria Souza   | Av. B, 456       | 10         | Caneta       | 5          | 10,00          |


### Normalização até a 3 Forma Normal(3FN)

## 1 Forma Normal
_- Eliminar repatições e garantir que cada campo tenha apenas um valor por registro_

| Cliente_ID | Cliente_Nome| Cliente_Endereço|
|-------------|-------------|-------------|
|      1      | Jõao Silva  | Rua A, 123  |
|      2      | Maria Souza |   Av.B,456  |

## 2 Forma Normal
_- Remover dependências parciais_

| Pruduto_ID | Produto_Nome | 
|-------------|-------------|
|  10         |  Caneta     | 
|  11         |  Lápis      | 

## 3 Forma Normal
_- Remover dependências transitivas_

|  Pedido_ID  | Produto_ID  | Quantidade  |  Preço_Total |
|-------------|-------------|-------------| -------------|
|  1          |   10        |      2      |     4,00     |
|  2          |   11        |      5      |     10,00    |
```json

{
  "pedido_id": 1,
  "cliente": {
    "nome": "João Silva",
    "endereco": "Rua A, 123"
  },
  "itens": [
    {
      "produto_id": 10,
      "nome": "Caneta",
      "quantidade": 2,
      "preco_unitario": 4.00,
      "preco_total": 8.00
    },
    {
      "produto_id": 11,
      "nome": "Lápis",
      "quantidade": 1,
      "preco_unitario": 2.00,
      "preco_total": 2.00
    }
  ]
},
{
  [
  "pedido_id":2,
  "cliente":{
   "cliente_id"2
   "nome": "Maria Souza"
   "endereco": "Av. B, 456"
   }
 ]
}


```












 
