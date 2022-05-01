# Counterfactual_Explanation_for_deep_learning
In the second part of the test, we will be using heart failure clinical record data set. We will be using artificial neural network and Bidirectional LSTM for prediction whether the patient survives or not and then we will be going forward with the counterfactual part of the implementation where we will be making our model explainable by in the case prediction made is that patient dies than a counter sequence of input is generated from which we can change the prediction to positive one (that he survives). The method we will be using for the counterfactual part will be 1 NN Baseline Method.
First part of the problem in my hand was prediction here I have used two different models a Neural Network and a Bidirectional LSTM.  After getting the prediction I will differentiate all the negative prediction with the positive predictions. Then I will be using an unsupervised Neural Network to fit our model with all the positive sequences of the values. Then using the closest neighbor to our negative prediction sequence using hamming distance model will predict the alternative counterfactual sequence to make the prediction positive.
We were able to complete all these parts and the files are attached with this document.
The Document consist of two models:
•	Heart_failure.ipynb
•	Lstm.ipynb
In the heart failure Jupiter notebook, I have implemented a Neural Network model to predict whether the person dies or not. In the end the counterfactual sequences will be discussed for the negative prediction sequences.
 In the later file that is the LSTM one I will be using a bidirectional LSTM to predict whether the person dies or not then for counter factual part 1 neural network base line will be used using hamming distance.

The Data set used is provided in kaggle and find the link for the data set below:

1.	Davide Chicco, Giuseppe Jurman: Machine learning can predict survival of patients with heart failure from serum creatinine and ejection fraction alone. BMC Medical Informatics and Decision Making 20, 16 (2020). (link)
