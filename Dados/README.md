
## Origem do Dataset
- **Fonte:** [Contoso Data Generator V2 - SQLBI](https://github.com/sql-bi/Contoso-Data-Generator-V2-Data)  
- **Período coberto:** 18/05/2021 a 20/04/2024  
- **Licença:** MIT License (uso comercial e não comercial permitido)  

## Metadados (Resumo)
O dataset contém múltiplas tabelas relacionadas ao varejo, entre elas:

- **Customer** → informações de clientes (nome, idade, localização, profissão, etc.)  
- **Orders** → dados de pedidos (data, cliente, loja, moeda, etc.)  
- **OrderRows** → detalhes de cada pedido (produto, quantidade, preço, custo, etc.)  
- **Product** → catálogo de produtos (nome, marca, categoria, preço, etc.)  
- **Sales** → vendas realizadas com valores brutos e líquidos  
- **Store** → informações das lojas (localização, área, status)  
- **Date** → calendário com hierarquia de datas  

## Tratamento
Os dados passaram pelas seguintes etapas:  
1. Limpeza de valores inconsistentes e duplicados (`scripts/limpeza_dados.R`).  
2. Seleção de colunas relevantes para análise exploratória.  
3. Consolidação no arquivo `dataset_tratado.csv` em `/dados/processado/`.  

