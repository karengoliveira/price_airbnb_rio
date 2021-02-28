# price_airbnb_rio
# Karen Regina - fev 2021

A partir da base de dados do Arirbnb do Rio de Janeiro buscou-se desenvolver um modelo para estimação de preço, baseado em algumas características da locação, de modo a auxiliar novos parceiros na precificação de seus espaços.

# Como foi a definição da sua estratégia de modelagem?
Considerando a natureza da variável resposta, a estratégia de modelagem foi direcionada para modelos de regressão linear múltipla. Buscou-se enfatizar a importância do tratamento dos dados que são utilizados na modelagem, de modo a permitir que o modelo obtido reflita com maior proximidade o cenário real e apresente desempenho satisfatório para aplicação.

# Como foi definida a função de custo utilizada?
Foi utilizado o algoritimo Light Boosting Gradient Model (LGBM), buscando a maximização do coeficiente de determinação (R²).

# Qual foi o critério utilizado na seleção do modelo final?
Foi realizada apenas uma ilustração de aplicação da técnica, não tendo sido aplicado tunning ao modelo, eliminando a necessidade de seleção de modelo final. Seriam avaliados os desempenhos de alguns modelos por meio do R² após testados alguns hiperparâmetros pré-selecionados, de modo que o modelo final escolhido seria aquele que apresentasse melhor desempenho.

# Qual foi o critério utilizado para validação do modelo? Por que escolheu utilizar este método?
Considerando o volume de dados disponíveis foi feita a utilização de 70% dos dados para treino e 30% dos dados para teste/validação do modelo. Optou-se pela realização de amostragem aleatória simples para a divisão da base, entretanto poderia ter sido realizada uma amostragem estratificada com base nas categorias das variáveis categóricas consideradas, de modo a garantir a representatividade dos cenários nas bases de treino e teste.

# Quais evidências você possui de que seu modelo é suficientemente bom?
A partir do R² é possível observar que cerca de 50% da variação do preço dos espaços pôde ser explicada a partir das variáveis selecionadas. Entretanto, na base de teste houve uma redução do R² de modo que seria necessário aprofundar o estudo para apresentar um modelo suficientemente bom para aplicação.

Considerando o objetivo proposto e também a concentração da diferença entre preço predito e observado em torno de zero, tanto para a base de treino como para a base de teste, entende-se que o resultado foi uma exemplificação coerente para apresentação da técnica.
