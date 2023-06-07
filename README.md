# Preprocessing and Commitee (PaC)

# Detalhes dos experimentos

## PaC para detectar intrusos no ToN-IoR Network multiclasse

### configuração do PaC utilizada nos experimentos do artigo
O PaC foi desenvolvido baseado na biblioteca `scikit learn`. Assim, todas as configurações apresentadas a seguir refletem os hiper-parâmetros presentes nas classes dessa bibliteca.  

configuração dos classificadores do PaC encontradas via `grid search`   
- `Random Forest` (RF)
  - criterion = log loss 
  - max depth = 8
  - max features = log2
  - min samples split = 4
  - n estimators = 300
- `Decision tree classifier` (DTC)
  - criterion = log loss
  - min samples split = 2
  - splitter = best
- `Multilayer perceptron` (MLP)
  - activation = tanh
  - alpha = 0.001 
  - hidden layer sizes = (100, 100)
  - learning rate = daptive
  - max iter = 200 
  - solver = adam
   
## PaC para detectar intrusos no ToN-IoR Devices binário/multiclasse 

Espaço de parâmetros utilizados para a busca via `grid search`   
- `Regressão Logística` (RL)
  - penalty = [l1, l2], 
  - C = [0.1, 1, 10], 
  - solve = [liblinear, saga, newton-cg, saga],
  - max iter = [100, 500, 1000], 
  - multi class = [ovr, multinomial], 
  - class weight = [None,balanced]
- `K-nearest neighbors` (KNN)
  - k neighbors = [1, 3, 5, 7, 9], 
  - metric = [euclidean, manhattan, chebyshev, minkowski]
- `Naice bayes` (NB)
  - alpha = [0.1, 0.5, 1.0
- `Linear Discriminant Analysis` (LDA)
  - solver = [svd, lsqr, eigen]
- `Random Forest` (RF)
  - n estimators = [100, 300, 500], 
  - max depth = [3, 5, 7], 
  - min samples split = [2, 5, 10], 
  - min samples leaf = [1, 2, 4], 
  - max features = [sqrt, log2], 
  - bootstrap = [True, False]
