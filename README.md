# Sistema de Pedidos - Factory Pattern

Este projeto implementa o **Factory Pattern** para criação de pedidos em Java.

## Como funciona

- `Pedido` → Interface base para todos os tipos de pedido.
- `PedidoOnline` → Implementação de pedidos online.
- `PedidoLojaFisica` → Implementação de pedidos na loja física.
- `PedidoFactory` → Fábrica responsável por criar instâncias dos pedidos.
- `Main` → Classe principal que demonstra o uso do Factory.

## Exemplo de uso

```java
Pedido pedido1 = PedidoFactory.criarPedido("online");
pedido1.processar();

Pedido pedido2 = PedidoFactory.criarPedido("loja");
pedido2.processar();


