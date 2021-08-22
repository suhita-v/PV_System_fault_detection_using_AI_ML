# PV_System_fault_detection_using_AI_ML
1.	What's this project about?
-	We propose an intelligent fault diagnosis model based on ANN (Artificial Neural Network) that uses multilayer perceptron (MLP) to accurately identify and classify the electrical faults in the photovoltaic module that is applicable in all environmental conditions on a grid-connected photovoltaic system.
2.	Which faults can be simulated?
-	Open Circuit
-	Short-Circuit
-	Degradation
-	Shading/ Shadow
3.	What is the PV System's description?
-	2 solar arrays of 50W, 12V each
-	Current Detection sensor module
-	Voltage Detection sensor module
-	Digital Light Intensity sensor
-	Temperature sensor
-	Arduino Uno
4.	Which software was used to simulate the hardware?	
- Proteus 8 Professional
5.	What's the software model?
-	We used SVM (Support Vector Machine) since it works the best on text classification problem. The dataset after being pre-processed was fed to various models such as: Random Forest, DecisionTree, KNeighbors and Gaussian. To avoid overfitting, data was divided in train and test in preprocesssing with train datapoint being 75% and training the model at the remainig 25%. Out of the classifiers used Decision tree, KNN and Random forest has shown promissing accuracies. With Random Forest leading with 99.8%. But the data being unbaised with many classes in the last 25%; hence it was required to shuffle the data randomly and split the data set in groups. Here, **k-fold Cross Validation** was done with k=10.
## Neural Networks-
-	We propose an intelligent fault diagnosis model for detecting faulty modules and further classifying the fault type that is applicable in all environmental conditions. The model uses the multilayer perceptron (MLP) and follows the supervised learning approach. It is robustly trained with historical data of different faulty and normal states in different environmental conditions especially focusing on winter. The data was collected from gird-connected PV system located in Portugal.
-	Accuracy of Multi-layer Perceptron with 30 Epochs came out 98.48%
-	To check the bias-variance tradeoff, a k-fold crossvalidation test is performed with the 5 validations split into the training data. Also, for improving the model and reducing overfitting, we implemented the dropout regularization technique. The dropout rates of 0.1 and 0.2 were selected for the first and second hidden layers, respectively.
-	Accuracy of MLP of 20 Epochs with cv = 5 came out 97.80
## Files-
-	Project.pptx contains an overview of the whole project undertaken
-	Software models of Machine learning and Deep learning
-	Dataset.zip contains the dataset acquired in CSV format
