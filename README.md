# Deep Learning Challenge

## Background
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

## Neural Network Model Report
1. Overview of the analysis: Explain the purpose of this analysis.
-  The purpose of this analysis is to see if an Alphabet Soup-funded organization will be successful based on the features in the dataset. 

2. Data Preprocessing
    - What variable(s) are the target(s) for your model?
        - The target for the model is the 'IS_SUCCESSFUL' column.
    - What variable(s) are the features for your model?
        - The features of the model include APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, and SPECIAL_CONSIDERATIONS. These features are featured after the unncessary columns of 'EIN' and 'NAME' were removed.
    - What variable(s) should be removed from the input data because they are neither targets nor features?
        - STATUS and SPECIAL_CONSIDERATIONS should be removed from the data because in the Status column they were the same value - 1 for Status, and SPECIAL_CONSIDERATONS because it is not a numerical data. 
* Compiling, Training, and Evaluating the Model
    - How many neurons, layers, and activation functions did you select for your neural network model, and why?
        - In the first attempt, with Layer 1 at 8 and Layer 2 at 5 and activation functions = relu, Loss: 0.5528853535652161, Accuracy: 0.7253644466400146.
            - Reference: Image 001.png in Images.
    - Were you able to achieve the target model performance?
        - No, I was unable to achieve the target model performance; achieved an accuracy of 72.5%.
    - What steps did you take in your attempts to increase model performance?
        - To increase model performance, I increased the hidden layers and change activation functions from relu to segmoid.
            - Reference: Image 002.png and Image 003.png

* Summary: Based on the overall results of the deep learning model, I was unable to achieve at least a 75% accuracy. I believe I should remove additional columns to the data frame and any columns that are not quanitifiable as they would take up space. Also, by changing the activation functions it could boost accuracy and help achieve at least a 75% accuracy. I don't believe adding additional hidden layers would help as it is more important to determine the number of neurons in the hidden layers versus listing additional hidden layers. Pruning a neural network will determine an optimal structure for a neural network.

