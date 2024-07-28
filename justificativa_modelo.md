### Justificativa para o Uso do Modelo de Regressão Linear

A escolha do modelo de regressão linear para prever o fechamento do índice Ibovespa foi baseada em várias considerações importantes, que são detalhadas a seguir:

#### 1. Simplicidade e Interpretação

O modelo de regressão linear é um dos métodos mais simples e interpretáveis em aprendizado de máquina. Sua natureza linear permite que os coeficientes do modelo sejam facilmente interpretados, fornecendo uma compreensão clara de como cada variável independente (feature) influencia a variável dependente (fechamento do Ibovespa). Esta interpretação é crucial para análise financeira, onde a transparência e a capacidade de explicar as previsões são altamente valorizadas.

#### 2. Eficiência Computacional

A regressão linear é computacionalmente eficiente e pode ser treinada rapidamente mesmo em datasets grandes, como o histórico de dados do Ibovespa. Este aspecto é especialmente importante quando se trata de prever fechamentos diários com um grande volume de dados.

#### 3. Bom Desempenho em Relações Lineares

Muitas relações econômicas e financeiras podem ser aproximadas por modelos lineares. Apesar de os mercados financeiros frequentemente exibirem comportamento complexo e não linear, a regressão linear pode capturar tendências gerais e padrões subjacentes nos dados. Adicionalmente, como o objetivo é prever fechamentos diários, onde as variáveis macroeconômicas e de mercado têm um impacto linear significativo, a regressão linear é uma escolha adequada.

#### 4. Robustez e Generalização

A regressão linear tende a ser robusta e generaliza bem em cenários com ruído e variação moderada nos dados. Isso é importante ao lidar com dados financeiros, que são conhecidos por sua volatilidade. Ao utilizar técnicas como a normalização das features e a remoção de outliers, o modelo de regressão linear pode oferecer previsões estáveis e confiáveis.

#### 5. Facilmente Extensível

A regressão linear pode ser facilmente estendida para incluir novas variáveis ou para se transformar em um modelo de regressão polinomial, se necessário. Essa flexibilidade permite que o modelo seja ajustado e melhorado conforme novos dados se tornam disponíveis ou conforme novas tendências emergem no mercado.

### Conclusão

Em resumo, o modelo de regressão linear foi escolhido para este projeto devido à sua simplicidade, eficiência computacional, capacidade de interpretar coeficientes, robustez e generalização. Embora existam modelos mais complexos que podem capturar não-linearidades nos dados, a regressão linear oferece uma base sólida para entender as tendências gerais e fazer previsões diárias do fechamento do índice Ibovespa.

A utilização deste modelo, portanto, é justificada pelas suas várias vantagens práticas e teóricas que atendem bem aos objetivos do projeto.
