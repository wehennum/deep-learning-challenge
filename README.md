# deep-learning-challenge
Overview:
The purpose of this analysis is to create a binary classifier using machine learning and neural networks. Alphabet Soup wants a model that"can help it select the applicants for funding with the best chance of success in their ventures". By leveraging features from a provided dataset, the goal is to create a model that can accurately classify whether applicants have a high probability of success if funded by Alphabet Soup. This predictive tool aims to optimize the foundation's decision-making process, ensuring that resources are allocated to ventures with the greatest potential for success. Alphabet Soup is aiming for an accuracy threshold of 75% in the model to ensure the reliability of the classifier in identifying successful applicants.

Results:
Data Preprocessing
Target Variable: The target variable used for the model is the column 'IS_SUCCESSFUL', which determines if the funding was used successfully by the applicant.
Feature Variables: The features for the model include is focused on IS_SUCCESSFUL.
Variables Removed: The EIN and NAME columns were removed as they do not factor into the model and are not needed 

Compiling, Training, and Evaluating the Model:
The initial neural network model consisted of an input layer with 80 neurons, a hidden layer with 30 neurons, and an output layer with a single neuron. The activation function 'tanh' was used for the input and hidden layers, and sigmoid for the output layer to suit the binary classification task. In the second optimization attempt, we changed the activation function to 'relu' and kept the neurons, hidden layer and output layer the same. In the third we went back to 'tanh' increased the input layer to 100 and kept everything the same. Despite these changes the model never reached the required accuracy of 75% only getting to 73% when we used the 'relu' method in the second attempt. 

Optimization
First attempt was optimized by adjusting the number of neurons in each hidden layer and selecting appropriate activation functions(tanh).These choices were made to enhance the model's ability to accurately predict the success likelihood of funding applicants for Alphabet Soup, aligning with the foundation's target accuracy of 75%. It did not reach the desired accuracy percentage
Second attempt we kept everything the same but switched the activation function to 'tanh' in hopes the model would reach the required accuracy percentage. It still fell short of the desired accuracy.
Third attempt we went back to 'tanh' activation and increased the first hidden layer from 80 up to 100. All three attempts to reach the desired accuracy of 75% fell short. We did come close getting the accuracy up to 73% but still came up a little short. 

While we did come close to achieving the desired accuracy we never reached it. Some things we could try to achieve the accuracy could be to use different machine learning models, adjusting the input layers more, deleting some columns of unneeded data. A mix of these things could take this model to where the client would want it to be., 
