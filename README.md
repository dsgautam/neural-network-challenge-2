# neural-network-challenge-2
Module 19 Homework Challenge

# Background:
You are tasked with creating a neural network that HR can use to predict whether employees are likely to leave the company. Additionally, HR believes that some employees may be better suited to other departments, so you are also asked to predict the department that best fits each employee. These two columns should be predicted using a branched neural network.

# Solution: 
The solution is included in the github directory "https://github.com/dsgautam/neural-network-challenge-2"
The solution was developed using Google Colab.

The steps takes are broadly defined here:

1. Data Preprocessing
2. Identifying the Target Columns
3. Selecting the Feature columns most relevant for the analysis
4. Convert categorical data into numerical data using relevant encoders
    - Label Encoders
    - One Hot Encoder
5. Splitting the Features and Targets into Training and Test datasets
6. Defining input  and hidden layers for the neural network
7. Compiling and executing the training model
8. Evaluting the results  on the testing dataset

Activation functions used:

1. Softmax Activation: Softmax is commonly used in multi-class classification problems where the network needs to output probabilities for each class.

2. Sigmoid Activation: Sigmoid activation function is often used in binary classification problems where the network needs to predict a binary outcome (0 or 1).

3. ReLU Activation: ReLU (Rectified Linear Unit) is a widely used activation function in hidden layers due to its simplicity and effectiveness. However, ReLU is not directly suitable for output layers in classification tasks because it doesn't bound the output values between specific ranges.

# Results: 
After executing the model, the testings results of the attrition prediction accuracy was high (~83%), whereas the prediction of the department accuracy was no better than a coin toss. The model can be further improved by one of the following techniques, if more time and resources are available.

**Architecture Design**: By tweaking the architecture layers of the model we can improve the performance.
  
  1. Deeper Networks: Increasing the depth of the network with additional layers can allow for more complex feature extraction and potentially better performance.
  
  2. Activation functions: By trying different activation functions, especially suited for branching and multi-task functions and comparing the results for accuracy and precision.

**Optimization Techniques**: We can use appropriate optimization techniques that might improve the results. For e.g. conducting systematic hyperparameter tuning, including parameters such as learning rate, dropout rates, batch sizes, and network architecture hyperparameters, can lead to improved performance.

**Ensemble Methods**: Combining predictions from multiple individual models, either with different architectures or trained on different subsets of data, can often yield better performance than a single model.

**Improving Data Class Imbalance**:  By reducing the imbalance across various data classes might help imrove the results of the model

**Additional Features**:  we used 10 columns in our feature selection. By using additional columns in the feature dataset, and checking the features most contributing to the performance and output of the model, we can hope to improve the results.







