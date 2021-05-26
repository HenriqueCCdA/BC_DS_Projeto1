# Notebooks exploratórios

# 1. Resumo
Nesta pasta estão os notebooks auxiliares do projeto

## 1.2. Lista de notebooks

* limpeza_de_dados_IPCA_INPC.ipynb
* Correcao_monetaria.ipynb
* Producao_hospitalar_com_correcao_monetaria.ipynb


# 3. [limpeza_de_dados_IPCA_INPC.ipynb](./Limpeze_de_dados_IPCA_INPC.ipynb)

Neste notebook os dados de IPCA e INPC são tratados. Os dados brutos de IPCA e INPC foram retirados do IBGE.

As fontes são: [IPCA](https://www.ibge.gov.br/estatisticas/economicas/precos-e-custos/9256-indice-nacional-de-precos-ao-consumidor-amplo.html?=&t=o-que-e) e [INPC](https://www.ibge.gov.br/estatisticas/economicas/precos-e-custos/9258-indice-nacional-de-precos-ao-consumidor.html?=&t=series-historicas)

O procedimento do tratamento foi o seguinte:

1. Dados brutos no formato .xls ([ipca_202104SerieHist.xls](../Dados/IBGE/ipca_202104SerieHist.xls))
2. Um pretramento feito atraves do excel ([ipca_202104SerieHist_mod.xls](../Dados/IBGE/ipca_202104SerieHist_mod.xls))
3. O tratamento feito no notebook 
4. Salvamento do arquivo tratado no formato .csv ([ipca.csv](../Dados/IBGE/ipca.csv))

Um explicação da diferença entre IPCA e INPC pode ser encontrado no proprio site do IBGE [IPCA vs INPC](https://www.ibge.gov.br/explica/inflacao.php#:~:text=A%20sigla%20INPC%20corresponde%20ao,uso%20do%20termo%20%E2%80%9Camplo%E2%80%9D.&amp;text=O%20INPC%20verifica%20a%20varia%C3%A7%C3%A3o,1%20a%205%20sal%C3%A1rios%20m%C3%ADnimos)

# 4. [Correcao_monetaria.ipynb](./Correcao_monetaria.ipynb)

Neste notebook é feito o procedimento de como fazer o calculo da correção monetária. Neste [video](https://www.youtube.com/watch?v=tFtk4BT2rdU) encontra-se uma explicação de como se fazer o calculo da correção monetária. O procedimento para o IPCA e INPC são os mesmo.  

Exemplo: 100 Reais em Janeiro de 2008 equivale a quanto em Dezembro de 2020 ?


Tabela IPCA
data     | indice
:----:   |:-----:
Jan/2008 | 2746.37
  ...   |  ... 
Jan/2020 | 5331.42

* Caclulo:

<p align="center">
<img src="https://render.githubusercontent.com/render/math?math=Valor_{corrigido} = Valor_{antigo} \times \frac{IPCA_{novo}}{IPCA_{antigo}}"> 
</p>

Usando os dados do exemplo:

<p align="center">
<img src="https://render.githubusercontent.com/render/math?math=Valor_{corrigido} = 100 \times \frac{5331.42}{2746.37} = 202.47"> 
</p>

Logo R$ 100 reais em Janeiro de 2008 equivale cerca R$ 202 em dezezembro de 2020.

