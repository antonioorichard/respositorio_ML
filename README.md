
# 1. Nome do Projeto
Ensaio de Machine Learning
# 2. Problema de Negócio
## 2.1 Descrição
A empresa Data Money acredita que a expertise no treinamento e ajuste fino dos algoritmos, feito
pelos Cientistas de Dados da empresa, é a principal motivo dos ótimos resultados que as
consultorias vem entregando aos seus clientes.
## 2.2 Objetivo
O objetivo desse projeto será realizar ensaios com algoritmos de Classificação, Regressão e
Clusterização, para estudar a mudança do comportamento da performance, a medida que os
valores dos principais parâmetros de controle de overfitting e underfitting são ajustados.
# 3. Planejamento da solução
## 3.1 Produto final
O produto final será 7 tabelas mostrando a performance dos algoritmos, avaliados usando múltiplas
métricas, para 3 conjuntos de dados diferentes: Treinamento, validação e teste.
## 3.2 Algoritmos ensaiados
**Classificação**:
**Algoritmos**             : KNN, Decision Tree, Random Forest e Logistic Regression
**Métricas de performance**: Accuracy, Precision, Recall e F1-Score


**Regressão**:
**Algoritmos**             : Linear Regression, Decision Tree Regressor, Random Forest Regressor, Polinomial
Regression, Linear Regression Lasso, Linear Regression Ridge, Linear Regression Elastic Net,
Polinomial Regression Lasso, Polinomial Regression Ridge e Polinomial Regression Elastic Net
**Métricas de performance**: R2, MSE, RMSE, MAE e MAPE.


**Agrupamento**:
**Algoritmos**             : K-Means e Affinity Propagation
**Métricas de performance**: Silhouette Score

## 3.3 Ferramentas utilizadas:
Python **3.12.0** e Scikit-learn, matplotlib, pandas, time e numpy.

# 4. Desenvolvimento
## 4.1 Estratégia da solução
Para o objetivo de ensaiar os algoritmos de Machine Learning, será utilizado a linguagem Python 
para escrever os códigos. Na etapa de treinamento cada um dos algoritmos é escrito com 
os seus principais parâmetros de ajuste de overfitting, e ainda com as principais métricas para observar o comportamento. O conjunto de valores que fizerem os algoritmos alcançarem a melhor performance, serão aqueles escolhidos para o treinamento final do algoritmo.


## 4.2 O passo a passo
**Passo 1**: Divisão dos dados em treino, teste e validação.
**Passo 2**: Treinamento dos algoritmos com os dados de treinamento, utilizando os parâmetros
“default”.
**Passo 3**: Medir a performance dos algoritmos treinados com o parâmetro default, utilizando o
conjunto de dados de treinamento.
**Passo 4**: Medir a performance dos algoritmos treinados com o parâmetro “default”, utilizando o
conjunto de dados de validação.
**Passo 5**: Alternar os valores dos principais parâmetros que controlam o overfitting do algoritmo até
encontrar o conjunto de parâmetros apresente a melhor performance dos algoritmos.
**Passo 6**: Unir os dados de treinamento e validação
**Passo 7**: Retreinar o algoritmo com a união dos dados de treinamento e validação, utilizando os
melhores valores para os parâmetros de controle do algoritmo.
**Passo 8**: Medir a performance dos algoritmos treinados com os melhores parâmetro, utilizando o
conjunto de dados de teste.
**Passo 9**: Avaliar os ensaios e anotar os 3 principais Insights que se destacaram.


# 5. Os top 3 Insights 
## 5.1 Insight Top 1 
Os algoritmos baseados em árvores possuem uma performance melhor em todas as métricas, quando aplicados sobre os dados de teste, no ensaio de Classificação. 
## 5.2 Insight Top 2
A performance dos algoritmos de classificação sobre os dados de validação ficou bem próxima da performance sobre os dados de teste, exceto com K-nn. 

## 5.3 Insight Top 3
 Todos os algoritmos de regressão e clusters não apresentaram boas métricas de performance, o que mostra uma necessidade de uma seleção de atributos e uma preparação melhor das variáveis independentes do conjunto de dados.

# 6. Resultados
## 6.1 Ensaio de Classificação ( Classification )

![Resultados da classificação](/Imagem/image.png)

## 6.2 Ensaio de Regressão     ( Regression )
### Parte I
![Resultados da regressão Parte I](/Imagem/image-1.png)
### Parte II
![Resultados da regressão Parte II](/Imagem/image-2.png)
### Parte III
![Resultados da regressão Parte III](/Imagem/image-3.png)

## 6.3 Ensaio de Agrupamento   (Clusters )
K-means             : 0.2305

Affinity Propagation: 0.2022

# 7. Conclusões
Nesse ensaio de Machine Learning, adquirir experiência sobree o funcionamento dos limites
dos algoritmos entre os estados de underffiting e overfitting. Deste modo, foi notado que os algoritmos baseados em árvores são sensíveis quanto a profundidade do crescimento e do número de árvores na floresta, fazendo com que a escolha correta dos valores desses parâmetros impeça os algoritmos de entrar no estado de overfitting ou underffitig. Já os algoritmos de regressão, são sensíveis ao grau do polinômio, de modo que esse parâmetro controla o limite entre o estado de underfitting e overfitting desses algoritmos.
Esse ensaio de Machine Learning foi importante para aprofundar o entendimento sobre o funcionamento de diversos algoritmos de classificação, regressão e clusterização, tendo os principais parâmetros de controle ajustes que podem levar ou tirar dos estados de underfitting e overfitting.
Por último, conclui-se que em alguns casos como de regressão e agrupamento, faz se necessário um estudo e preparo maior do conjunto de dados, já que não foi encontrado resultado satifatório em nenhum modelo.

# 8. Próximos passos
Para próximos passo, incluir novos algoritmos e Machine Learning e usar diferentes conjuntos de dados para aumentar o conhecimento sobre os algoritmos e quais cenários são mais favoráveis para o aumento da performance dos mesmos.



# CURSO MACHINE LEARNING EM PYTHON
Este projeto foi criado com víeis acadêmicos para o curso de fundamentos de Machine Learning. 

