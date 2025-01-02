# Previsão de Ações com RNN

Este projeto utiliza redes neurais recorrentes (RNN) para prever os preços futuros de ações com base em dados históricos de diversas ações e do mercado em geral. O modelo é treinado usando o PyTorch e os dados são extraídos com a ajuda da biblioteca `yfinance`.

## Objetivo

O objetivo deste projeto é desenvolver uma rede neural para prever o preço de fechamento ajustado das ações com base em dados históricos. As previsões são feitas utilizando uma janela de 10 dias de cotações passadas como features para prever o valor do preço de fechamento ajustado no próximo dia.

## Tabela de Conteúdos

- [Sobre](#sobre)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Como Instalar](#como-instalar)
- [Como Usar](#como-usar)
- [Estrutura de Dados](#estrutura-de-dados)
- [Modelo de Previsão](#modelo-de-previsão)
- [Contribuindo](#contribuindo)
- [Licença](#licença)

## Sobre

O projeto busca utilizar dados financeiros de ações brasileiras e de mercado para prever os preços futuros de fechamento das ações. As informações são extraídas através da API `yfinance`, onde são coletados os preços históricos de ativos selecionados, como:

- **Ações brasileiras**: SUZB3.SA, EMBR3.SA, PETR4.SA, EGIE3.SA, entre outras.
- **Índice Bovespa**: ^BVSP.
- **Cotação do dólar**: USDBRL=X.

A partir destes dados, são criadas janelas de 10 dias para serem usadas como entradas para o modelo RNN. O objetivo final é usar esses dados para prever os preços ajustados das ações no dia seguinte.

## Tecnologias Utilizadas

- **Python 3.12.3**
- **yfinance**: para obter dados históricos de ações.
- **NumPy**: para manipulação eficiente de arrays.
- **PyTorch**: para construção e treinamento do modelo de rede neural recorrente (RNN).
- **Pandas**: para manipulação e análise de dados.
- **Matplotlib / Seaborn** (opcional): para visualização de resultados.

## Como Instalar

Clone este repositório para a sua máquina local:

```bash
git clone https://github.com/gabriels3t/Uso-de-RNN-para-prever-acoes.git
