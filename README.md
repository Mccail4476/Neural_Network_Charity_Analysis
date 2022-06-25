# Neural_Network_Charity_Analysis


***Overview***

The purpose of this module is to demonstrate the use of basic Neural Networks to have a better trained machine learning model. Different model setups yield different outcomes, such as having multiple hidden layers & having multiple nodes per hidden layer. By applying these models to our data, we can better predict the outcome with improved accuracy by training the model with previous relevant data.


***Results***

*What variable(s) are considered the target(s) for your model?*

The targetted variable is the "Is Successful" in the dataset because this show which charities had a positive outcome. 


*What variable(s) are considered to be the features for your model?*

Featured variables of interest seem to be "Application Type" and "Classfication". 



*What variable(s) are neither targets nor features, and should be removed from the input data?*


Variables that provided little to no value would be:
-EIN
-Name
-Status
-Special Considerations

Though a true way of deciding how well the data correlates could be determine through use of unsupervised machine learning to see which had the lease correlation coefficient. R can also be used to determine which variable had the least amount of impact.


*How many neurons, layers, and activation functions did you select for your neural network model, and why?*

To improve the model to achieve the 75% threshold, I increase the number of hidden layers to hold 4 instead of 2. For all hidden layers, I used 8 nodes. Lastly, the activation function for all input hidden layers still used "Relu". Generally speaking, increasing the hidden layers and nodes per hidden layers is expected to improve the accuracy at the cost of increase computer resources and risk of overfitting. Furthermore, I decided to leave the activation function of "Relu" because linear, sigmoid, and tanh did seem to performed worse than "Relu". 

The output layer activation function was changed from sigmoid to linear to see if that would improve results.


*Were you able to achieve the target model performance?*

Unfortunately, I was not able to improve the model to achieve the 75% targetted performance. This doesn't mean that the model cannot achieve it, but the three limits I used were not sufficient. Though it is possible to ram-jam the different hidden layers, nodes, and activation to achieve this performance, this isn't the best use of time. The best approach is to have a deep understanding of what the model is doing in order to figure out how to best troubleshoot it. 


*What steps did you take to try and increase model performance?*

First attempt was to increse the number of hidden layers to see if that improved accuracy; It didn't.
Second attempt was to increse the number of nodes including first attempt changes; Barely increased the accuracy. 
Third attempt was to change the activation functions of the input and output layer including the deletion of data from the original dataset of the previously mentioned variables that didn't provide value; Increased yield of 1% from the original module yield.


***Summary***

The final yield after three attempts of optimization has left us with a 71% accuracy with a 59% loss of data. This isn't a terrible model but there is always room for improvement. A key takeaway is that it is important to remove variables that provide little to no value to training model so the machine learning model does not get bogged down by meaningless data. A recommendation I would do to further improve the model is to use unsupervised machine learning model to see what variables are important so I know to keep them. I would then delete all other variables and move forward with the training and testing phase. Another recommendation is to study the concept of what's happening on a deeper level. 
