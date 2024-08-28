# Análise de Dados - Veículos Nissan
Este projeto consiste em uma análise exploratória de dados utilizando um dataset fictício relacionado a uma loja de veículos Nissan. O objetivo é responder a perguntas específicas sobre desempenho de vendas, segmentação de mercado, condição dos veículos, quilometragem, preço e perfil dos clientes.

## 1. Dataset
O dataset utilizado foi baixado do Kaggle e contém dados **fictícios** diversas sobre modelos de veículos Nissan, incluindo preços, quilometragem, condição dos veículos, além de dados demográficos dos clientes.

1.1 Fonte do dataset:
* [Nissan All Models Price Prediction Dataset](https://www.kaggle.com/datasets/marius2303/nissan-all-models-price-prediction-dataset)

1.2 Ferramentas Utilizadas:
* Linguagem Python e suas bibliotecas: Pandas, Plotly.express e Matplotlib.pyplot
* Muito importante mencionar aqui que utilizei primeiramente o Plotly.express para gerar os gráficos por ser mais dinâmico e ser possível interagir com ele, contudo, o GitHub não suporta a exibição dos gráficos do Plotly.express, devido a isso refiz os gráficos utilizando a biblioteca Matplotlib.pyplot, por conta disso no código você verá dois blocos de código antes do gráfico.
  
1.3 Estrutura do Projeto
* Carregamento do dataset e inspeção inicial da estrutura.
* Análise de valores ausentes e criação de colunas de faixa (ranges) para dados como idade, performance, quilometragem e preço.
  
1.4 Análise e Visualização:
* Desenvolvimento de gráficos interativos para auxiliar nas análises e a responder às perguntas de negócio. A preferência pela utilização do Plotly.express é justamente pelo dinamismo dos gráficos gerados por essa biblioteca.
* Exploração dos dados com foco em insights que auxiliem a identificar pontos críticos e em tomadas de decisões.

## 2. Objetivos da Análise

2.1 Desempenho de Vendas:
* Identificar o modelo de carro mais vendido.
* Analisar se há uma correlação entre a performance do veículo e o preço.

2.2 Segmentação de Mercado:
* Determinar a faixa etária dos clientes que mais compram carros.
* Verificar se há preferência por cores de carros entre diferentes gêneros.

2.3 Condição do Veículo e Preço:
* Avaliar como a condição do carro afeta o preço de venda.
* Calcular a média de preços para carros em diferentes condições (ex: very bad, bad, old, very good).
  
2.4 Quilometragem e Preço:
* Investigar a correlação entre a quilometragem do carro e o preço de venda.
* Analisar a quilometragem média dos carros vendidos em diferentes faixas de preço.

2.5 Perfil Demográfico dos Clientes:
* Explorar a distribuição de gênero dos compradores.
* Identificar a faixa etária mais comum dos compradores de cada modelo de carro.


## 3. Conclusões com base nas Perguntas Iniciais:

3.1 Impacto da Condição do Veículo no Preço:
* Com base na análise realizada, podemos constatar que não **há praticamente nenhuma correlação entre performance e preço**. Além disso, podemos verificar com essa análise que a maioria esmagadora dos veículos, independetemente de performance, se mantém na faixa do $50.000.

3.2 Correlação Entre Quilometragem e Preço:
* Nessa análise novamente foi possível observar que há uma correlação muito fraca entre as variáveis "km" e "price", mostrando que não há um padrão que interfira para que o preço distoe de um veículo para os demais.

3.3 Segmentação de Mercado por Faixa Etária:
* A maior parte dos clientes estão concentrados na faixa etária entre 46 e 60 anos, explicitando que este grupo é um segmento de mercado importante para a loja com 49,42% de compras a mais que a faixa etária na segunda colocação que é entre 36 e 45 anos. Portanto, se agruparmos as duas faixas etárias o range ficaria entre 36 e 60 anos, e esse grupo representa 49,69% de toda a base de dados.

3.4 Preferências de Cor por Gênero:
* Com base na análise feita e a utilização do gráfico, podemos verificar que **não há uma cor de veículo que possamos considerar uma preferência absoluta.** Dentre os gêneros, é claro que a **cor vermelha é a que possui mais busca entre os homens** e a **prata entre as mulheres**, no entanto, chama a atenção a baixa procura por algumas cores e devido a isso vamos alterar a forma de ver o gráfico trazendo apenas a quantidade de compras por cor, sem os gêneros.

3.5 Modelo de Veículo Mais Vendido:
* Foi identificado que o modelo de veículo mais vendido nessa base de dados é o **Juke** com **882** vendas.
