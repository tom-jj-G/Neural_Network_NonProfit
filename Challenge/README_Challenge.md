# Challenge

## How many neurons and layers did you select for your neural network model? Why?

x2 neurons by input because best practice
1 layer to save computation resources, increase speed and avoid overfitting 


## Were you able to achieve the target model performance? What steps did you take to try and increase model performance?

If yes: great !

if not, try :
    - x3 neuros by imput
    - additional layers
    - increase epochs


## If you were to implement a different model to solve this classification problem, which would you choose? Why?

Random forest classifiers(Scikit-Learn’s *RandomForestClassifier*) as it might be equally performant and handle non-linear data well.
Additionaly, both Scikit-Learn’s RandomForestClassifier class and TensorFlow’s Sequential class require preprocessing, so prepocessing stpes could be keep.