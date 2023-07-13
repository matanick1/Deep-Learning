                                ANALYSIS OF CHARITY FUNDING

1.	Purpose of the analysis: 

    •	Alphabet Soup wants a tool that can help it select which applicants for funding have the best chance of success.

2.	Results:

    •	Data Preprocessing

    1.	What variable(s) are the target(s) for your model? 
    
        	I used “IS_SUCCESSFUL” as the target variable.

    2.	What variable(s) are the features for your model? 
    
    
        	APPLICATION_TYPE

        	AFFILIATION

        	CLASSIFICATION

        	USE_CASE

        	ORGANIZATION

        	STATUS

        	INCOME_AMT

        	SPECIAL_CONSIDERATIONS

        	ASK_AMT

    3.	What variable(s) should be removed from the input data because they are neither targets nor features? 

        	“EIN” and “NAME”

    •	Compiling, Training, and Evaluating the Model

    4.	How many neurons, layers, and activation functions did you select for your neural network model, and why?

        	For the first model, I used 2 hidden layers with 80 and 30 neurons. I chose 80 and 30 because it is roughly twice the number of input features. I used “relu” activation function for the hidden layers and “sigmoid” for the output layer. I used “binary_crossentropy” for the loss function and “adam” for the optimizer.

    5.	Were you able to achieve the target model performance? 

        	No, I got to just over 74%, but never reached 75%.

    6. 	What steps did you take in your attempts to increase model performance?

        	I added a third hidden layer.

        	I changed the neurons in all of the layers to 100, 50, and 25.

        	I reduced the number of epochs to 50.


3.	Summary: 
    1.	The optimized model ended up having a slightly better accuracy than the optimized model. The original model had an accuracy of 72.52% and the optimized model had an accuracy of 72.53%.

    2.	I would use the Keras Tuner library to try to make my model because it provides a streamlined and efficient way to search for the best hyperparameters for my model.
