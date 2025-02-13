# analise-pdfs-politicas
Scripts para extração e consolidação de políticas públicas em PDFs
# Análise de PDFs de Políticas Públicas

Este repositório contém scripts para extração e consolidação de dados de políticas públicas a partir de arquivos PDF.

## 📌 Funcionalidades
1. **`processar_pdf.py`** - Analisa arquivos PDF de leis orçamentárias, buscando políticas especificadas em um arquivo Excel e gerando um CSV com os resultados.
2. **`consolidar_dados.py`** - Mescla os dados extraídos com uma base qualitativa de políticas, consolidando as informações em um arquivo final.

## 📂 Estrutura do Repositório
```
📂 analise-pdfs-politicas/
│── 📂 scripts/
│   ├── processar_pdf.py          # Script para processar PDFs
│   ├── consolidar_dados.py       # Script para consolidar dados extraídos
│── .gitignore                    # Arquivos a serem ignorados no repositório
│── README.md                     # Documentação do projeto
```

## 🚀 Como Usar

### 1️⃣ **Pré-requisitos**
Certifique-se de ter **Python 3.x** instalado. Instale as bibliotecas necessárias:
```bash
pip install pdfplumber pandas openpyxl chardet
```

### 2️⃣ **Execução dos Scripts**
#### **Processar os PDFs**
Coloque os arquivos PDFs na pasta desejada e execute:
```bash
python scripts/processar_pdf.py
```
Digite o ano do PDF que deseja analisar quando solicitado.

#### **Consolidar os Dados**
Após gerar os arquivos CSV, execute:
```bash
python scripts/consolidar_dados.py
```

O arquivo consolidado será salvo automaticamente.

## 🛑 .gitignore
O arquivo `.gitignore` evita o upload de arquivos desnecessários ao repositório:
```
__pycache__/
*.csv
*.xlsx
checkpoint_*.txt
```


