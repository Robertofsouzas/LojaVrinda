# LojaVrinda

Este projeto tem como objetivo realizar uma análise completa dos dados da LojaVRinda, desde a coleta até a visualização de insights utilizando o Amazon QuickSight.

![Pipeline]![ETL](https://github.com/Robertofsouzas/LojaVrinda/assets/67076322/fff492d3-2c4a-4cc3-ac98-b6ceba708461)

# Passo 1 Carregando as Bibliotecas
- **import os
- **import pandas as pd
- **import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from datetime import datetime
import time
import pymssql as sql
import warnings
warnings.filterwarnings("ignore")
import pyodbc
import sqlalchemy as sa 
import openpyxl
from scipy.stats import skew
from kaggle.api.kaggle_api_extended import KaggleApi

# Passo 2: Coleta de Dados no Kaggle

Vá para o Kaggle e encontre o conjunto de dados relevante da LojaVRinda.(https://www.kaggle.com/datasets/anshika2301/vrinda-store-data-analysis)

Conectei via API

# Passo 3: Carregando os Dados para o Amazon S3 (Camada Raw)
Crie um bucket no Amazon S3.

Utilize a AWS CLI para carregar o conjunto de dados no seu bucket do S3.

# Passo 4 Análise Exploratória


# Passo 5: Tratamento e Limpeza dos Dados

usei  o Jupyter Notebook.

Utilizei bibliotecas como Pandas para carregar e manipular os dados.

Realizei a limpeza dos dados, tratando valores ausentes e outliers, engenharia de atributos.


# Passo 6: Análise Estatística Descritiva

No Jupyter Notebook, utilizei ferramentas como Pandas e Matplotlib/Seaborn para realizar análises estatísticas descritivas para identificar padrões e tendências.



# Passo 7: Encontrando Insights

> 1. Diferença de Gênero nas Compras:
As mulheres apresentam uma probabilidade 65% maior de fazer compras em comparação aos homens.

> 2. Principais Estados em Vendas:
Maharashtra, Karnataka e Uttar Pradesh destacam-se como os três principais estados em volume de vendas.

> 3. Contribuição por Faixa Etária:
O grupo de idade adulta (30-49 anos) é o que mais contribui, representando uma contribuição de 50%.

>4. Principais Canais de Venda:
Aprimorado: Os canais de venda Amazon, Flipkart e Myntra são os principais contribuintes, representando 80% do total de vendas



# Passo 8: Carregando os dados tratados e limpos para o s3 camada gold

usando a Configurações do AWS ,  Configurações do Amazon S3 , Configuração do cliente S3



# Passo 9: Visualização no Amazon QuickSight

Acesse o Amazon QuickSight.

 conectei o conjunto de dados na camada "gold" do S3 ao Quicksight

Desenvolvi um dashboards visualmente atraentes utilizando os insights obtidos.

Publique seu dashboard no QuickSight para compartilhamento e acesso fácil.


# Conclusão Final:
Direcione campanhas de marketing para mulheres na faixa etária de 30 a 49 anos, residentes em Maharashtra, Karnataka e Uttar Pradesh, destacando anúncios, ofertas e cupons disponíveis nos canais de venda da Amazon, Flipkart e Myntra.




![Dashboard_LojaVrinda]![Dashboard_lojaVrinda](https://github.com/Robertofsouzas/LojaVrinda/assets/67076322/3dca334c-cdaa-4ad9-8677-76bd9d17be67)






