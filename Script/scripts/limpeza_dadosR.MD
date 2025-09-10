# Script de Limpeza de Dados - Projeto Aplicado I

# Carregar pacotes necessários
library(dplyr)
library(readr)

# Ler dados brutos (ajuste o caminho se necessário)
dados <- read_csv("../dados/bruto/csv-10k/Sales.csv")

# Exemplo de limpeza: remover duplicados e NAs
dados_limpos <- dados %>%
  distinct() %>%
  na.omit()

# Salvar dataset tratado
write_csv(dados_limpos, "../dados/processado/dataset_tratado.csv")

print("✅ Limpeza concluída e dataset_tratado.csv gerado com sucesso!")

