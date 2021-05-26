# Notebooks exploratórios

# 1. Resumo
Nesta pasta estão os notebooks auxiliares do projeto

## 2. Lista de notebooks

* Correcao_monetaria.ipynb
* Producao_hospitalar_com_correcao_monetaria.ipynb
* limpeza_de_dados_IPCA_INPC.ipynb

# 3. limpeza_de_dados_IPCA_INPC.ipynb [open](./Correcao_monetaria.ipynb)

Neste notebook os dodos de IPCA e INPC são tratados. Os dados brutos de IPCA e INPC foram retirados do IBGE.

As fontes são: [IPCA](https://www.ibge.gov.br/estatisticas/economicas/precos-e-custos/9256-indice-nacional-de-precos-ao-consumidor-amplo.html?=&t=o-que-e) e [INPC](https://www.ibge.gov.br/estatisticas/economicas/precos-e-custos/9258-indice-nacional-de-precos-ao-consumidor.html?=&t=series-historicas)

O procedimento do tratamento foi o seguinte:

1. Dados brutos no formato .xls ([ipca_202104SerieHist.xls](../Dados/IBGE/ipca_202104SerieHist.xls))
2. Um pretramento feito atraves do excel ([ipca_202104SerieHist_mod.xls](../Dados/IBGE/ipca_202104SerieHist_mod.xls))
3. O tratamento feito no notebook 
4. Salvamento do arquivo tratado no formato .csv ([ipca.csv](../Dados/IBGE/ipca.csv))

Um explicação da diferença entre IPCA e INPC pode ser encontrado no proprio site do IBGE [IPCA vs INPC](https://www.ibge.gov.br/explica/inflacao.php#:~:text=A%20sigla%20INPC%20corresponde%20ao,uso%20do%20termo%20%E2%80%9Camplo%E2%80%9D.&amp;text=O%20INPC%20verifica%20a%20varia%C3%A7%C3%A3o,1%20a%205%20sal%C3%A1rios%20m%C3%ADnimos)
