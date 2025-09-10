# Script de Análise Exploratória - Projeto Aplicado I

# Carregar pacotes
library(dplyr)
library(readr)
library(ggplot2)

# Ler dados tratados
dados <- read_csv("../dados/processado/dataset_tratado.csv")

# Exemplo 1: vendas por mês
vendas_por_mes <- dados %>%
  group_by(OrderDate = format(as.Date(OrderDate), "%Y-%m")) %>%
  summarise(total_vendas = sum(NetPrice, na.rm = TRUE))

# Gráfico de vendas por mês
ggplot(vendas_por_mes, aes(x = OrderDate, y = total_vendas)) +
  geom_line(color = "blue") +
  labs(title = "Vendas por Mês", x = "Mês", y = "Total de Vendas") +
  theme_minimal()

# Salvar gráfico
ggsave("../resultados/gráficos/vendas_por_mes.png", width = 8, height = 5)

print("✅ Análise exploratória concluída e gráfico salvo!")
