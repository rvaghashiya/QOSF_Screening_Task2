# QOSF Screening Task 2: Encoding and Classifier

# Aim
* Encoding the following data (mock_train_set.csv and mock_test_set.csv ) in a quantum circuit in at least two different ways (these could be basis, angle,  amplitude, kernel or random encoding).
* Design a variational quantum circuit for each of the encodings, uses the column 4  as the target,  this is a binary class 0 and 1.
* You must  use the data from column0 to column3 for your proposed classifier. 
* Consider the ansatz you are going to design as a layer and find out how many layers are necessary to reach the best performance.


# Method
* Data pre-processing
* Quantum Embedding of the classical data 
* Train a layered variational quantum classifier


# Data Embedding methods
* Amplitude Embedding
* Angle Embedding


# Framework:
* PennyLane


## Dataset: 
* mock_train_set.csv
* mock_test_set.csv


# Result Analysis and Discussion

It is observed that with an increase in the number of layers in the variational classifier, there is an increase in the classification performance with a smoother convergence. The performance gain saturates at the third layer. 
For the optimizer in use, Adam, a learning rate of $0.1$ leads to a faster initial convergence while the performance is unstable and saturates quickly. 
With a learning rate of $0.01$, the classifier has a slower but smoother convergence and a stable performance gain.

The best performance of $95.83\%$ is achieved for variational classifier using amplitude-encoding.
