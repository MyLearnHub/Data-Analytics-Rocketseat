# Coletando dados com SQL

## O que é um banco de dados relacional?

- Armazena dados em tabelas organizadas com linhas e colunas
- Cada tabela representa uma entidade: clientes, produtos, vendas...
- As tabelas se conectam por colunas em comum → relacionamento

## O que é SQLite?

- Um banco de dados leve e embutido
- Ideal para testes, ensino e análises locais
- Usa arquivos `.db` ou funciona direto na memória
- Muito usado com Python + pandas + dashboards simples

## Por que usar SQLite?

- Permite testar tudo que precisa aprender em SQL
- Roda sem precisar de servidor, internet ou conta de banco
- Pode simular vários casos reais (vendas, clientes, produtos...)
- Não tem ambientes complexos de infraestrutura

Ideal para aprender SQL com foco em análisede dados

## Entendendo SELECT e WHERE

- `SELECT` = o que você quer ver
- `WHERE` = qual condição aplicar

Exemplo:
Quero ver o nome e cidade dos clientes que são de SP

```sql
SELECT nome, cidade FROM clientes WHERE cidade = 'SP'
```

## Onde o SQL entra na prática nas empresas?

- 🔍 Dashboards: dados vêm de SQL antes de virar gráfico
- 📊 BI (Power BI, Tableau): se conectam com bancos e fazem queries
- 🤖 Automação de relatórios: scripts em Python que usam SQL
- 🧾 Extração de dados de sistemas: CRM, ERP, e-commerces
