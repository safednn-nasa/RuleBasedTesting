# Rule-Based-Testing

This repository contains code to demonstrate the use of rules extracted from a DNN model, to be used as oracles to label new data and a coverage criteria to evaluate test-suites. The notebook Rule_Based_Test_Oracle_Coverage_MNIST.ipynb demonstrates these applications on MNIST using a CNN model with ReLU activations. The 60K train set is used to extract rules for correct classification to each of the 10 labels, and mis-classification. The rules are validated on a validation set with 5k inputs and the rules with precision > 80% are chosen for the applications. A test set with 5k inputs are used to evaluate the efficacy of the selected rules i) to act as oracles to make two types of predictions for every input a) whether the model is likely to produce a correct output , b) the ground-truth label, and ii) act as a coverage criteria to rank test-suites according to functional diversity, feature diversity and defect detection ability.
