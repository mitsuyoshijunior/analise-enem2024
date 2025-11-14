# Arquivos Processados - ENEM 2024

Esta pasta contém os arquivos processados do ENEM 2024 utilizados nos notebooks e análises do projeto.

Devido ao tamanho dos arquivos, eles não estão incluídos diretamente no repositório. Para utilizar os notebooks, siga os passos abaixo:

---

## Como usar os arquivos

1. Baixe os arquivos processados da pasta do Google Drive do projeto  para o seu próprio Drive ou computador:

https://drive.google.com/drive/folders/13Lgj5xFCcurwLE6OfsIYdXdvvT5jkI9B?usp=drive_link

2. Copie o **caminho completo do arquivo** que você baixou.

3. No notebook, substitua o valor da variável `caminho` pelo caminho que você copiou.  
   Exemplo:

```python
caminho = "/content/drive/MyDrive/analise-diagnostico-enem2024/data/processed/RESULTADOS_2024_processed.csv"
import pandas as pd

df = pd.read_csv(caminho, sep=";", encoding="latin-1")
df.head()
