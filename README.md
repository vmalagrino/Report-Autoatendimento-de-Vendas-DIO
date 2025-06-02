# Self-Service Report de Vendas
Focado em documentar o processo de estudo da análise de dados rápidas e individuais das bases de dados de vendas com ajuda do ChatGPT (Versão gratuita).
## Prompts
Foi solicitado ao chat analisar nossos arquivos de vendas dos 3 ditribuidores em modelo CSV. 
Com base nisso recebemos alguns insights do modelo de IA:

- Receita total por plataforma e por país
- Produtos mais vendidos
- Descontos médios aplicados
- Distribuição de vendas por mês
- Análise por faixa etária dos compradores
- Conversão de moedas (se necessário para comparação realista entre plataformas)

## Racional feito pelo modelo em Python

import pandas as pd

Carregar os três arquivos CSV
aliexpress_df = pd.read_csv("/mnt/data/Meganium_Sales_Data_-_AliExpress.csv")
etsy_df = pd.read_csv("/mnt/data/Meganium_Sales_Data_-_Etsy.csv")
shopee_df = pd.read_csv("/mnt/data/Meganium_Sales_Data_-_Shopee.csv")

Exibir as 5 primeiras linhas de cada DataFrame para análise inicial
aliexpress_preview = aliexpress_df.head()
etsy_preview = etsy_df.head()
shopee_preview = shopee_df.head()

aliexpress_preview, etsy_preview, shopee_preview

