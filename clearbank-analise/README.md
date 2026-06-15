# ClearBank Análise Financeira

Projeto desenvolvido em Python para leitura, validação e análise de transações bancárias a partir de um arquivo CSV.

## Objetivo

O notebook lê o arquivo `transacoes.csv`, valida os dados, remove registros inválidos, calcula métricas financeiras mensais, identifica transações suspeitas e exporta o resultado em JSON.

## Como executar

1. Abra o arquivo `desafio-final.ipynb` no Google Colab ou Jupyter Notebook.
2. Execute todas as células em ordem.
3. O notebook irá gerar o relatório no terminal e criar os arquivos de saída.

## Arquivo de entrada

- `transacoes.csv`

## Arquivos gerados

- `relatorio.json`: relatório final em formato JSON.
- `grafico.png`: gráfico com o saldo mensal.

## Funcionalidades

- Leitura de CSV com `csv.DictReader`
- Validação de dados
- Tratamento de erros com `try/except`
- Agrupamento mensal
- Cálculo de crédito, débito, saldo, média, maior e menor valor
- Identificação de transações suspeitas acima de R$ 10.000,00
- Exportação em JSON
- Geração de gráfico com matplotlib
