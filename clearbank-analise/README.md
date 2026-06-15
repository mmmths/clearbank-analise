# ClearBank - Análise Financeira com Python

Projeto desenvolvido para o desafio final de análise financeira com Python.

O notebook lê um arquivo `transacoes.csv`, valida os registros, descarta linhas inválidas, agrupa as transações por mês, calcula métricas financeiras, sinaliza transações suspeitas acima de R$ 10.000,00 e exporta o resultado em JSON.

## Arquivos do projeto

- `desafio-final.ipynb`: notebook principal com a solução.
- `transacoes.csv`: arquivo de teste com 15 registros válidos e 5 inválidos.
- `relatorio.json`: arquivo gerado pelo notebook com o resultado da análise.
- `grafico.png`: gráfico opcional com o saldo mensal.

## Como executar

1. Abra o arquivo `desafio-final.ipynb` no Google Colab ou Jupyter Notebook.
2. Execute todas as células em ordem.
3. Confira a saída formatada do relatório no notebook.
4. Verifique os arquivos gerados: `relatorio.json` e `grafico.png`.

## O que o notebook faz

- Lê o CSV usando o módulo nativo `csv` e `csv.DictReader`.
- Trata `FileNotFoundError` caso o CSV não exista.
- Valida `id`, `cliente_id`, `data`, `tipo` e `valor`.
- Usa `datetime.strptime` para validar e converter datas.
- Agrupa as transações por mês no formato `AAAA-MM`.
- Calcula total de créditos, total de débitos, saldo, média, maior valor e menor valor.
- Lista transações suspeitas com valor acima de R$ 10.000,00.
- Exporta o relatório final em `relatorio.json`.
- Gera o gráfico `grafico.png` com `matplotlib`.
