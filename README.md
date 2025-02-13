# analise-pdfs-politicas
Scripts para extração e consolidação de políticas públicas em PDFs
# Análise de Dados de Políticas Públicas

Este repositório contém notebooks para análise e consolidação de dados de políticas públicas extraídos de arquivos PDF.

## 📌 Conteúdo

1. **`Analise 2019-2024.ipynb`** - Notebook que processa arquivos PDF de projetos de leis orçamentárias e identifica políticas públicas mencionadas.
2. **`Consolidacao_dados_19_24.ipynb`** - Notebook que combina os dados extraídos dos PDFs com uma base qualitativa, consolidando as informações.

## 📂 Estrutura do Repositório
```
📂 analise-pdfs-politicas/
│── 📂 notebooks/
│   ├── Analise 2019-2024.ipynb   # Notebook para análise dos dados extraídos
│   ├── Consolidacao_dados_19_24.ipynb  # Notebook para consolidação dos dados
│   │── analise_politica.ipynb  # Notebook para analise de dados
│── .gitignore                    # Arquivo para ignorar arquivos desnecessários
│── README.md                     # Documentação do projeto
```
## 📊 Bases de Dados

Os arquivos de dados utilizados neste projeto estão disponíveis na pasta [`dados/`](./dados/):

- **politicas.xlsx** - Base contendo as políticas analisadas.
- **consolidado_politicas.csv** - Arquivo consolidado com informações sobre as políticas.
- **politicas-base-organizada.csv** - Base qualitativa com detalhes adicionais das políticas.
- **arquivos dos PLOAS.pdf** ( consultar e gerar no SIOP)

⚠️ **Os arquivos de saída gerados pelos notebooks (`resultado_YYYY.csv`, `consolidado_politicas_atualizado.csv`) não estão no repositório**, pois podem ser gerados ao rodar os notebooks.

## 🚀 Como Usar

### 1️⃣ **Pré-requisitos**
Certifique-se de ter **Python 3.x** instalado. Instale as bibliotecas necessárias executando:
```bash
pip install pdfplumber pandas openpyxl chardet
```

### 2️⃣ **Execução dos Notebooks**

#### **Analisar PDFs**
Coloque os arquivos PDFs na pasta desejada e abra o notebook:
```bash
jupyter notebook notebooks/Analise 2019-2024.ipynb
```
Siga as instruções dentro do notebook para processar os arquivos.

#### **Consolidar os Dados**
Após extrair os dados dos PDFs, abra o notebook para consolidar os resultados:
```bash
jupyter notebook notebooks/Consolidacao_dados_19_24.ipynb
```
#### **Consolidar os Dados**
Após consolidação, analisar dados.
```bash
jupyter notebook notebooks/analise_politica.ipynb

`````````

## 🛑 .gitignore
O arquivo `.gitignore` evita que arquivos temporários ou grandes sejam adicionados ao repositório:
```
__pycache__/
*.csv
*.xlsx
checkpoint_*.txt
*.ipynb_checkpoints/
```





