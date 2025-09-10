## 📘 Relatório – Projeto Aplicado I
## 1. Título do trabalho

Análise Exploratória de Dados: Performance da Varejista Fictícia Contoso, uma abordagem em R.

## 2. Membros do grupo

Bruna Graciano

Guilherme Marques Gomes dos Santos

Sophia Pereira Ramos

## 3. Contexto do estudo

O presente trabalho tem como objetivo realizar uma Análise Exploratória de Dados (AED) sobre a performance da varejista fictícia Contoso.
A análise considera aspectos de vendas e métricas operacionais, buscando gerar insights relevantes para a tomada de decisão, como lucro obtido, custos associados e o comportamento dos clientes.

## 4. Cronograma de execução
Etapa	Atividade	Entregável	Prazo
1	Apresentação do projeto, objetivos, metas e milestones	Kick Off	04/09
2	Definição do produto analítico e análise exploratória	Proposta + AED	16/10
3	Apresentação de produtos (resultados e storytelling)	Relatório intermediário	13/11
4	Encerramento do projeto	Projeto final	27/11
5. Organização no GitHub

## 📂 Estrutura de pastas

projeto_aplicado_I/
│
├── README.md
├── docs/
│   ├── relatorio.md
│   └── figuras/
│       ├── diagrama_sales.png
│       └── diagrama_orders.png
├── data/
│   ├── raw/
│   │   └── csv-10k/
│   └── processed/
│       └── dataset_tratado.csv
├── scripts/
│   ├── analise_exploratoria.R
│   └── limpeza_dados.R
├── resultados/
│   ├── graficos/
│   │   ├── vendas_por_mes.png
│   │   ├── lucro_operacional.png
│   │   └── perfil_clientes.png
│   └── tabelas/
│       └── resumo_kpis.csv
└── LICENSE


## 📌 Descrição:

docs/ → Relatório e figuras utilizadas.

data/ → Dataset bruto e processado.

scripts/ → Códigos em R para limpeza e análise.

resultados/ → Gráficos, tabelas e outputs da análise.

README.md → Explicação do projeto no GitHub.

6. Referência de aquisição do dataset

Origem: SQL BI - Contoso Data Generator V2 - Data

Período: 18/05/2021 a 20/04/2024

Licença: MIT License (uso livre para fins acadêmicos e comerciais)

## 7. Descrição da origem

O dataset foi criado pela Microsoft para demonstração de ferramentas de Business Intelligence (BI).
Ele simula dados de uma grande rede de varejo e é amplamente utilizado em projetos acadêmicos e de treinamento.

## 8. Objetivo do trabalho

Mensurar KPIs de vendas (volume vendido, receita, lucro).

Analisar performance operacional (custos, margens, eficiência de lojas).

Explorar comportamento do cliente (perfil de compra, idade, localização).

Com base nisso, o trabalho busca levantar hipóteses e responder perguntas estratégicas sobre a performance da varejista.

## 9. Descrição do dataset

O dataset contém várias tabelas relacionais no formato de estrela (star schema), com destaque para:

Sales → informações de vendas.

Orders → pedidos realizados.

Customer → dados de clientes.

Product → catálogo de produtos.

Store → informações de lojas.

Date → calendário de referência.

As chaves de cruzamento entre tabelas permitem análises multidimensionais (por produto, cliente, tempo, loja etc.).

📊 Exemplos de atributos:

Customer: idade, gênero, cidade, profissão.

Product: nome, categoria, fabricante, preço, custo.

Sales: quantidade, preço unitário, custo unitário, data da venda.

## 10. Metodologia

Aquisição do dataset (pasta /data/raw/).

Limpeza e tratamento dos dados (script limpeza_dados.R).

Análise exploratória:

Identificação de KPIs.

Geração de tabelas resumo.

Construção de gráficos descritivos.

Documentação dos resultados em /resultados/.

Construção do Data Storytelling no relatório.

## 11. Resultados esperados

Gráficos de evolução das vendas ao longo do tempo.

Comparativo de margem de lucro por produto e loja.

Perfil dos clientes (idade, gênero, localização).

Indicadores consolidados em tabelas resumo.

## 12. Conclusão

A análise exploratória do dataset Contoso permitirá compreender melhor os fatores que impactam a performance do varejo, auxiliando em decisões estratégicas relacionadas a vendas, custos e comportamento do cliente.
