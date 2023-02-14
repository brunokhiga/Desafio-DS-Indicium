DESAFIO INDICIUM - DATA SCIENCE
Objetivo:
O desafio proposto neste processo seletivo consiste na modelagem de um Machine Learning cujo objetivo é identificar quais máquinas apresentam potencial de falha. 
Para isso foram fornecidas duas bases de dados, uma para treino do modelo e outra para teste.

Dados:
As bases de dados possuem 8 colunas de dados possuem as seguintes variáveis:
- UID: unique identifier ranging from 1 to 10000
- product ID: consisting of a letter L, M, or H for low (50% of all products), medium (30%) and high (20%) as product quality variants and a variant-specific serial number
- type: just the product type L, M or H from column 2
- air temperature [K]: generated using a random walk process later normalized to a standard deviation of 2 K around 300 K
- process temperature [K]: generated using a random walk process normalized to a standard deviation of 1 K, added to the air temperature plus 10 K.
- rotational speed [rpm]: calculated from a power of 2860 W, overlaid with a normally distributed noise
- torque [Nm]: torque values are normally distributed around 40 Nm with a SD = 10 Nm and no negative values.
- tool wear [min]: The quality variants H/M/L add 5/3/2 minutes of tool wear to the used tool in the process.

Além destas, a base utilizada para treinamento do modelo possui a coluna failure_type, que indica a não ocorrência ou o tipo de falha ocorrida.
A base de dados para treinamento possui 6667 linhas.
A base de dados para teste possui 3333 linhas.

Ferramentas:
O problema foi resolvido em Python, utilizando o Jupyter Notebook.
As bibliotecas utilizadas foram: 
- pandas
- numpy
- matplotlib
- sklearn

Arquivos:
O repositório possui os seguintes arquivos:
- readme.txt: arquivo explicativo do projeto
- requirements.txt: bibliotecas a serem instaladas
- CaseML.ipynb: arquivo python da resolução do desafio
- predicted.csv: arquivo csv com o resultado obtido pelo machine learning
- desafio_manutencao_preditiva_teste.csv: arquivo csv para teste do modelo
- desafio_manutencao_preditiva_treino.csv: arquivo csv para treinamento do modelo
- Relatório Desafio DS.pdf: explicação mais detalhada do desenvolvimento e pontos de melhoria da resolução deste desafio.

Resultados:
Como explicado no arquivo 'Relatório Desafio DS', não consegui realizar testes eficácia para o modelo.
Quando realizado um teste com a base de dados para treinamento, utilizando 80% para o treinamento do modelo e 20% para teste, foi obtida uma acurácia de cerca de 97%.

Melhorias:
Análise de possíveis outliers e exclusão destes valores.
Comparação dos resultados obtidos pelo modelo com os resultados esperados pelos valores das variáveis.
Realizar testes para verificar a confiabilidade do modelo.

Autor: Bruno Kenhy Higa


 