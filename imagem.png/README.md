# Modelagem de Dados Ecommerce
# Modelo Conceitual - Sistema de Gestão de Pedidos e Serviços

## Descrição do Projeto

Este projeto tem como objetivo apresentar um modelo conceitual de banco de dados para um sistema que gerencia pedidos, clientes (PF e PJ), formas de pagamento, entregas e ordens de serviço com responsáveis.

O diagrama foi criado utilizando a ferramenta [draw.io](https://draw.io), seguindo boas práticas de modelagem de dados. Ele contempla as entidades principais envolvidas no processo de atendimento e entrega de pedidos, além do relacionamento com serviços associados e seus respectivos responsáveis.

## Objetivos do Desafio

O modelo foi refinado para atender os seguintes requisitos:

- **Cliente PF e PJ**: Um cliente pode ser Pessoa Física (CPF) ou Pessoa Jurídica (CNPJ), mas nunca ambos.
- **Pagamento**: Um pedido pode ter múltiplas formas de pagamento associadas.
- **Entrega**: Cada pedido possui um status de entrega e um código de rastreio associado.
- **Ordem de Serviço**: Associada a pedidos e com responsáveis definidos.
- **Relacionamentos adicionais**: Inclusão de tabelas auxiliares para representar relacionamentos N:N (muitos para muitos), como `Pedido_Pagamento` e `Responsavel_Ordem`.

## Entidades Principais

- **Cliente**: Contém dados básicos e se relaciona com `Cliente_PF` ou `Cliente_PJ`.
- **Pedido**: Ligado ao cliente e utilizado para registrar os dados de compra.
- **Forma de Pagamento**: Possui os métodos cadastrados e se relaciona com pedidos através da tabela `Pedido_Pagamento`.
- **Entrega**: Guarda status e código de rastreio.
- **Ordem de Serviço**: Contém a descrição de serviços relacionados a pedidos.
- **Responsável**: Usuário atribuído a uma ordem de serviço.
- **Tabelas auxiliares**: `Pedido_Pagamento` e `Responsavel_Ordem` representam relacionamentos muitos-para-muitos.

## Diagrama

O diagrama está disponível no formato `.drawio` neste repositório com o nome:  
**modelo_conceitual_modelagem_dados_ecommerce.drawio**

---

