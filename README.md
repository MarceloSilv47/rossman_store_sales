# 1. Problema de negócio 

A Rossmann é uma rede de farmácia que tem diversas lojas físicas. Mas embora a rede seja grande e produza muitos dados diariamente, o CFO (Chef Financial Officer) da empresa resolveu destinar uma verba para reformar apenas algumas lojas. 

Para ter noção do quanto que vai poder investir em cada uma das lojas, ele precisa de uma estimativa do quanto cada uma irá vender nas próximas 6 semanas em relação ao período em questão, sendo assim, foi solicitado ao time de dados uma previsão de vendas do quanto cada loja iria vender no determinado período. 

# 2. Premissas do negócio 

1. A análise foi realizada com dados entre 01/01/2013 e 21/07/2015. 
2. Uma rede de varejo foi o modelo de negócio assumido.

# 3. Estratégia da solução 

Para resolver o problema da Rossmann em questão foi usado um passo a passo que vai desde a descrição dos dados, passa pela criação de hipóteses, análise exploratória e preparação dos dados, seleção de variáveis e termina com os testes nos algoritmos de machine learning e a interpretação dos erros para o plano do negócio.

Foram levantadas diversas hipóteses, todas foram analisadas sob diversas óticas com análises gráficas e analíticas, algumas  foram validadas e outras não. Na preparação dos dados, foram usados métodos de reescala com o robustscaler e minmaxscaler e de transformação de variáveis categóricas em numéricas, como o one hot encoding, o label encoding e o ordinal encoding.

Para a seleção de features foi usado o algoritmo Boruta que trouxe as melhores variáveis para os testes com os algoritmos de machine learning. Já nos testes dos algoritmos de machine learning foram explorados os modelos: Linear Regression, Linear Regression Regularized, Forest Regressor e o XGBoost.

O XGBoost foi escolhido como modelo após analisar a performance dos modelos com o MAE (Mean Absolute Error), MAPE (Mean Absolute Percentage Error) e RSME (Root Mean Squared Error).

# 4. Top 3 Insights de dados 

1. Lojas com maior sortimento de produtos não vendem mais.
2. Lojas com promoções ativas por mais tempo não vendem mais.
3. Lojas vendem menos durante os feriados escolares.

# 5. O produto final do projeto

Bot no Telegram hospedado no render em que o usuário digita o número da loja e recebe a previsão estimada das próximas 6 semanas. O bot pode ser acessado através desse link: https://t.me/ross_store_bot

# 6. Conclusão 

O objetivo desse projeto foi criar uma previsão de vendas de 6 semanas para a rede de farmácia Rossmann. Portanto, com o bot no Telegram pronto, é possível afirmar que o objetivo do projeto foi alcançado.

# 7. Próximo passos  

1. Prever vendas para um intervalo variável de acordo com o usuário.
2. Prever o valor que pode ser investido em na reforma de cada loja.
3. Acrescentar o erro percentual no bot do telegram.


