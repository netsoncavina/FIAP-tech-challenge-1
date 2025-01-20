# Análise de Dados de Seguros

Este projeto realiza uma análise exploratória e preditiva de um conjunto de dados de seguros. O objetivo é explorar os dados, realizar visualizações e aplicar modelos de regressão para prever os custos de seguro com base em variáveis independentes.

---

## Demonstração do Projeto

Clique na imagem abaixo para assistir ao vídeo no YouTube:  

[![Demonstração no YouTube](https://img.youtube.com/vi/lIPXVBnZ4YM/0.jpg)](https://www.youtube.com/watch?v=lIPXVBnZ4YM)


## Estrutura do Projeto

### 1. Importação de Bibliotecas
As seguintes bibliotecas são utilizadas neste projeto:
- **pandas**: Manipulação de dados.
- **matplotlib** e **seaborn**: Visualizações.
- **sklearn**: Modelos de aprendizado de máquina e métricas de avaliação.

### 2. Importação e Análise do Dataset
- O conjunto de dados `insurance.csv` é carregado usando `pandas`.
- Informações iniciais como primeiros registros, descrição, e verificação de valores nulos são realizadas.

### 3. Pré-processamento de Dados
Variáveis categóricas são codificadas usando `LabelEncoder`:
- `sex`: Codificado como 0 (female) e 1 (male).
- `smoker`: Codificado como 0 (não fumante) e 1 (fumante).
- `region`: Codificado em valores inteiros representando as regiões.

### 4. Análise de Correlação
A correlação entre variáveis é visualizada com um mapa de calor:

### 5. Visualizações
- Comparação do custo médio de seguro entre fumantes e não fumantes.
- Relação entre o índice de massa corporal (BMI) e os custos de seguro.

### 6. Modelagem Preditiva
Foram aplicados três modelos:

#### 6.1 Regressão Linear
O modelo linear básico foi treinado e avaliado usando as métricas MSE, MAE e R².

#### 6.2 Regressão Polinomial
Regressão polinomial de grau 2 foi implementada para capturar não linearidades nos dados.

#### 6.3 Random Forest
Um modelo de regressão baseado em florestas aleatórias foi aplicado para melhorar a precisão preditiva.

### 7. Avaliação dos Modelos
As seguintes métricas foram calculadas para cada modelo:
- **Mean Squared Error (MSE)**
- **Mean Absolute Error (MAE)**
- **R² Score**

### 8. Resultados
Os resultados das predições foram comparados visualmente e numericamente com os valores reais, fornecendo insights sobre a eficácia dos modelos.
* O modelo Linear Regression com Polynomial Features demonstrou desempenho superior ao modelo Linear Regression simples, evidenciando que a inclusão de termos polinomiais pode capturar melhor as não-linearidades presentes nos dados.
* O desempenho do modelo Linear Regression com Polynomial Features foi próximo ao do Random Forest, indicando que modelos mais simples, quando ajustados corretamente, podem competir com algoritmos mais complexos dependendo da natureza dos dados e do problema.
