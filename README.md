# Análise e Previsão do Fechamento do Ibovespa

Este projeto realiza uma análise exploratória dos dados históricos do Ibovespa e utiliza um modelo de regressão linear para prever os fechamentos futuros do índice. O projeto é dividido em cinco notebooks principais:

1. `preparacao_dados.ipynb`
2. `analise_exploratoria.ipynb`
3. `modelo_preditivo.ipynb`
4. `analise_impactos_economicos.ipynb`

## Estrutura do Projeto

```plaintext
meu_projeto/
│
├── preparacao_dados.ipynb
├── analise_exploratoria.ipynb
├── modelo_preditivo.ipynb
├── analise_impactos_economicos.ipynb
├── dados_preparados.csv
└── dados-historicos-ibovespa.csv
```

### 1. Preparação dos Dados (`preparacao_dados.ipynb`)

Neste notebook, carregamos os dados históricos do Ibovespa, realizamos a limpeza e a preparação dos dados. As etapas principais incluem:

- Importar bibliotecas necessárias.
- Carregar os dados históricos do Ibovespa.
- Converter a coluna `Data` para o formato datetime.
- Tratar valores faltantes preenchendo-os com a média.
- Criar novas features, incluindo a transformação logarítmica do volume e a criação de dummies para eventos econômicos específicos.
- Salvar os dados preparados em um novo arquivo CSV (`dados_preparados.csv`).

### 2. Análise Exploratória dos Dados (`analise_exploratoria.ipynb`)

Neste notebook, realizamos a análise exploratória dos dados históricos do Ibovespa. As etapas principais incluem:

- Importar bibliotecas necessárias.
- Carregar os dados preparados.
- Converter a coluna `Data` para o formato datetime.
- Identificar e remover outliers utilizando o método do IQR (Interquartile Range).
- Plotar gráficos para visualizar o fechamento diário, o volume diário e a variação percentual diária do Ibovespa ao longo do tempo.

### 3. Modelagem Preditiva (`modelo_preditivo.ipynb`)

Neste notebook, utilizamos um modelo de regressão linear para prever o fechamento do Ibovespa. As etapas principais incluem:

- Importar bibliotecas necessárias.
- Carregar os dados preparados.
- Preparar os dados para a modelagem, normalizando as features.
- Dividir os dados em conjuntos de treino (70%) e teste (30%).
- Treinar o modelo de regressão linear.
- Fazer previsões nos dados de teste e calcular o erro quadrático médio (MSE) e a acurácia do modelo.
- Plotar as previsões do modelo comparadas aos valores reais do fechamento do Ibovespa.

### 4. Análise do Impacto dos Eventos Econômicos (`analise_impactos_economicos.ipynb`)

Neste notebook, exploramos a relação entre eventos econômicos importantes e as variações no fechamento do índice Ibovespa. As etapas principais incluem:

- Importar bibliotecas necessárias.
- Carregar os dados preparados.
- Remover outliers utilizando o método do IQR (Interquartile Range).
- Visualizar a distribuição dos dados ao longo do tempo.
- Explorar o impacto de eventos econômicos específicos utilizando gráficos de boxplot.
- Calcular estatísticas descritivas para o fechamento do Ibovespa durante períodos de eventos econômicos.

### Como Executar o Projeto

#### 1. Clone este repositório para sua máquina local.

#### 2. Certifique-se de ter as bibliotecas necessárias instaladas. Você pode instalar as dependências utilizando o seguinte comando:
```plaintext
pip install pandas numpy scikit-learn matplotlib seaborn
```

#### 3. Execute os notebooks sequencialmente:
- preparacao_dados.ipynb
- analise_exploratoria.ipynb
- modelo_preditivo.ipynb
- analise_impactos_economicos.ipynb

