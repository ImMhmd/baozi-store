# Baozi Store - API REST

API REST simples (Java 17 + Spring Boot + Spring Data JPA + H2/MySQL) para controle de clientes, produtos e pedidos.

## Como rodar
    mvn spring-boot:run
ou importe como projeto Maven na IDE e execute `BaoziStoreApplication`.

A API sobe em http://localhost:8080

## Endpoints
| Recurso  | POST      | GET (listar) | GET por ID      | DELETE          |
|----------|-----------|--------------|-----------------|-----------------|
| Cliente  | /clientes | /clientes    | /clientes/{id}  | /clientes/{id}  |
| Produto  | /produtos | /produtos    | /produtos/{id}  | /produtos/{id}  |
| Pedido   | /pedidos  | /pedidos     | /pedidos/{id}   | /pedidos/{id}   |

## Exemplos de JSON
Cliente: {"nome": "SeuNome123456", "clienteDesde": "2026-11-23"}
Produto: {"nome": "Baozi de Carne", "preco": 8.50, "estoque": true}
Pedido:  {"clienteId": 1, "produtoId": 1, "quantidade": 3}
