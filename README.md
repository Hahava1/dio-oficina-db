# Projeto de Banco de Dados - Oficina Mecânica

Este projeto tem como objetivo modelar o banco de dados para um sistema de controle e gerenciamento de ordens de serviço (OS) em uma oficina mecânica. A modelagem segue uma narrativa realista de fluxo de atendimento de clientes, desde o cadastro até a execução dos serviços mecânicos.

---

## Objetivo

Criar um esquema conceitual que represente o processo completo de uma oficina mecânica, incluindo:

- Cadastro de clientes e seus veículos.
- Emissão de ordens de serviço.
- Designação de equipes e mecânicos.
- Execução de serviços com cálculo baseado em mão-de-obra.
- Utilização de peças com valores associados.
- Controle de status e prazos das ordens.

---

## Entidades Principais

- **Cliente**: Responsável por levar o veículo à oficina.
- **Veículo**: Carro ou moto do cliente que precisa de reparo ou revisão.
- **Ordem de Serviço (OS)**: Documento que reúne as informações do conserto.
- **Equipe**: Grupo de mecânicos responsável por avaliar e executar os serviços.
- **Mecânico**: Funcionário com especialidade que pertence a uma equipe.
- **Serviço**: Tipo de mão-de-obra cadastrada com valor de referência.
- **Peça**: Componente físico necessário para a execução dos reparos.

---

## Relacionamentos

- Um **cliente** pode ter **vários veículos**.
- Um **veículo** pode ter **várias ordens de serviço**.
- Uma **ordem de serviço** é atribuída a uma **equipe**.
- Uma **equipe** possui **vários mecânicos**.
- Uma **ordem de serviço** pode incluir **vários serviços** e **várias peças**.
- Os serviços e peças são cadastrados em tabelas próprias e são relacionados à OS por tabelas intermediárias com quantidade.

---

## Tabelas Associativas

- **ServicoExecutado**: Relaciona os serviços com cada OS.
- **PecaUtilizada**: Relaciona as peças com cada OS.

---

## Ferramentas Utilizadas

- **Draw.io**: Utilizado para criação do diagrama entidade-relacionamento (ER).
- **Modelo Conceitual**: Representa as entidades e seus relacionamentos.
- **Modelo Lógico** *(opcional)*: Conversão para formato com chaves primárias e estrangeiras.

---
