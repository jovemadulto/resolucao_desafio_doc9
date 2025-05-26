# Resolução do Desafio Técnico — Cientista de Dados Sênior · Doc9

## 👀 Introdução
Este é um desafio que consiste em apresentar soluções práticas a partir de dados fictícios extraídos de uma das bases da empresa [Doc9](https://doc9.com.br/) para sustentar decisões de quatro áreas distintas de negócios:
- Produto
- Operações
- Jurídico
- Executivo

Cada área de negócio apresentou questões distintas entre si, ao passo em que foram criados quatro arquivos diferentes, no formato Jupyter Notebook para respondê-las. O código utilizado foi preservado como forma de fundamentar estas respostas como recurso metodológico.

Também foi criada uma apresentação para a área Executiva com problemas observados durante a análise e recomendações para que estes vícios fôssem sanados de forma razoável.

---

## 📂 Estrutura do projeto

```
├── README.md                       # Instruções gerais do desafio
├── data/
│ └── solicitacoes_doc9.csv         # Base de dados fictícia
| └── limpo_solicitaccoes_doc9.csv  # Base de dados preparada para análise
├── data_to_report/
│ └── distribuicao_lead_time.csv    # Tabelas usadas para dataviz
│ └── solic_dias_semana.csv         # com ferramenta externa
│ └── leadtime_sem_outliers_menores.csv  
│ └── solicitacoes_por_dia.csv
│ └── solicitacoes_por_semana.csv
│ └── tabela_problemas_uf.csv
│ └── taxa_problemas_uf.csv
├── notebooks/
│ └── 01_exploracao.ipynb           # Análises exploratórias (obrigatório)
│ └── 02_produto.ipynb              # separadas por categorias de negócio
│ └── 03_operacoes.ipynb                
│ └── 04_juridico.ipynb             
│ └── 05_executivo.ipynb                
├── reports/
│ └── report_executivo.pdf          # Relatório Executivo (obrigatório)
├── models/
│ └── modelo_churn.py               # Modelo preditivo (opcional)
├── pipeline/
│ └── transformacoes.py             # Scripts de ETL ou transformação (opcional)
├── requirements.txt                # Dependências Python
└── .gitignore
```

---

## 🐍  Preparo do ambiente
O ambiente foi preparado utilizando a distribuição Miniconda em razão de sua conveniência e usabilidade.

Para copiar os arquivos, criar o ambiente e instalar as dependências necessárias, execute os seguintes comando no emulador de terminal.
```
git clone https://github.com/jovemadulto/resolucao_desafio_doc9.git
conda create --name desafiodoc9 --file requirements.txt`
conda activate desafiodoc9
```