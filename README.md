# LojaVrinda

Este projeto tem como objetivo realizar uma análise completa dos dados da LojaVRinda, desde a coleta até a visualização de insights utilizando o Amazon QuickSight.


# Passo 1: Coleta de Dados no Kaggle

Vá para o Kaggle e encontre o conjunto de dados relevante da LojaVRinda.(https://www.kaggle.com/datasets/anshika2301/vrinda-store-data-analysis)

Conectei via API

# Passo 2: Carregando os Dados para o Amazon S3 (Camada Raw)
Crie um bucket no Amazon S3.

Utilize a AWS CLI para carregar o conjunto de dados no seu bucket do S3.


# Passo 3: Tratamento e Limpeza dos Dados

usei  o Jupyter Notebook.

Utilizei bibliotecas como Pandas para carregar e manipular os dados.

Realizei a limpeza dos dados, tratando valores ausentes e outliers, engenharia de atributos.


# Passo 4: Análise Estatística Descritiva

No Jupyter Notebook, utilizei ferramentas como Pandas e Matplotlib/Seaborn para realizar análises estatísticas descritivas para identificar padrões e tendências.



# Passo 5: Encontrando Insights

1. Diferença de Gênero nas Compras:
As mulheres apresentam uma probabilidade 65% maior de fazer compras em comparação aos homens.

> 2. Principais Estados em Vendas:
Maharashtra, Karnataka e Uttar Pradesh destacam-se como os três principais estados em volume de vendas.

> 3. Contribuição por Faixa Etária:
O grupo de idade adulta (30-49 anos) é o que mais contribui, representando uma contribuição de 50%.

>4. Principais Canais de Venda:
Aprimorado: Os canais de venda Amazon, Flipkart e Myntra são os principais contribuintes, representando 80% do total de vendas



# Passo 6: Carregando os dados tratados e limpos para o s3 camada gold

usando a Configurações do AWS ,  Configurações do Amazon S3 , Configuração do cliente S3



# Passo 6: Visualização no Amazon QuickSight

Acesse o Amazon QuickSight.

 conectei o conjunto de dados na camada "gold" do S3 ao Quicksight

Desenvolvi um dashboards visualmente atraentes utilizando os insights obtidos.

Publique seu dashboard no QuickSight para compartilhamento e acesso fácil.


# Conclusão Final:
Direcione campanhas de marketing para mulheres na faixa etária de 30 a 49 anos, residentes em Maharashtra, Karnataka e Uttar Pradesh, destacando anúncios, ofertas e cupons disponíveis nos canais de venda da Amazon, Flipkart e Myntra.




![Dashboard_LojaVrinda](https://github.com/Robertofsouzas/LojaVrinda/issues/1](https://private-user-images.githubusercontent.com/67076322/290214020-4efd9dac-3241-40d3-9ac2-80e25f56cd3a.jpeg?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTEiLCJleHAiOjE3MDI0NzY4NDksIm5iZiI6MTcwMjQ3NjU0OSwicGF0aCI6Ii82NzA3NjMyMi8yOTAyMTQwMjAtNGVmZDlkYWMtMzI0MS00MGQzLTlhYzItODBlMjVmNTZjZDNhLmpwZWc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBSVdOSllBWDRDU1ZFSDUzQSUyRjIwMjMxMjEzJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDIzMTIxM1QxNDA5MDlaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1lMTFjZTY4MDIwOTJkYjE3Mjk4ZTI3MTAxZGU4MGU2MDIwYzVmZWNmMWM0ZjFiZGJlZDhmNmM0NTg5NTgxYzJhJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.UnfLzExI781dNUkBRfz2TIMyV0UB9qTPBTwOcOQ4AVQ)https://private-user-images.githubusercontent.com/67076322/290214020-4efd9dac-3241-40d3-9ac2-80e25f56cd3a.jpeg?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTEiLCJleHAiOjE3MDI0NzY4NDksIm5iZiI6MTcwMjQ3NjU0OSwicGF0aCI6Ii82NzA3NjMyMi8yOTAyMTQwMjAtNGVmZDlkYWMtMzI0MS00MGQzLTlhYzItODBlMjVmNTZjZDNhLmpwZWc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBSVdOSllBWDRDU1ZFSDUzQSUyRjIwMjMxMjEzJTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDIzMTIxM1QxNDA5MDlaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1lMTFjZTY4MDIwOTJkYjE3Mjk4ZTI3MTAxZGU4MGU2MDIwYzVmZWNmMWM0ZjFiZGJlZDhmNmM0NTg5NTgxYzJhJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.UnfLzExI781dNUkBRfz2TIMyV0UB9qTPBTwOcOQ4AVQ)






