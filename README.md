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
   
