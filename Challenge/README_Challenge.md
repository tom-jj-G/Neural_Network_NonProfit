# Challenge

## How many neurons and layers did you select for your neural network model? Why?

Neurons number has been selected to be twice as the number of features as per best practices.
As our number of inputs/features is 33, we have created 66 neurons. 

One layer has been created to save computation resources, increase speed and avoid potential overfitting. 


## Were you able to achieve the target model performance? What steps did you take to try and increase model performance?

Unfortunately, our first model achieved a poor performance with an accuracy of about 56%.
According to the loss and accuracy charts (cf. *AlphabetSoupChallenge.ipynb* file), we almost already reached the horizontal asymptote of our model, given us limited hope to improve our model. But we tried anyway!

We choose to:
1. Increase the number of neurons, equal to third time the number of features (maximum of what best pratices recommend): 99 total neurons
2. Add an additional layer of neurons, with the same number as the number of features (33)
3. Increase the number of epochs to 100 to train our model a little bit longer
4. Finally, we tried to remove some noisy data

After our last step, and as unfortunately forecasted, we barely improved our model with a final poor accuracy score of 57%.
Activation functions for hidden layers (*relu*) and output layer (*sigmoid*), loss function (*binary_crossentropy*) and optimizer function (*adam*) chosen seem to be the appropriate ones to analyze potential non-linear data with a binary classification required at the end (either a good or a bad use of the money gave to a organization).

The data might need to be cleaned a little bit more and/or we might need to delete some inputs/features.
Non-documented attempts with limited inputs/features did not increase the accuracy, they even ended up with a worst final accuracy score.


## If you were to implement a different model to solve this classification problem, which would you choose? Why?

If we had to choose a different model, a Random forest classifier model (using Scikit-Learn’s *RandomForestClassifier* method) could be used as it might be equally performant and handle pretty well non-linear data.
Additionally, both Scikit-Learn’s RandomForestClassifier class and TensorFlow’s Sequential class require preprocessing, so preprocessing steps could be kept.

After a non-documented attempt, a Random forest classifier model achieved a accuracy score equivalent to our neural model (56%), leading us with the thought that our data need additional selection with maybe potential features/inputs to drop.
