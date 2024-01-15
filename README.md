Introduction: 
My goal was to build an image classifier for differentiating pictures of cats vs. dogs. Furthermore, I wanted to evaluate the performance of LDA, QDA, and Closest Average decision rules for this task. 


Data: 
The dataset consisted of 64 x 64 grayscale images of 1000 cats and 1000 dogs.
The images are registered so facial features appear in the same region for each image.


Data Preprocessing:
Data Transformation:
Each picture was “unwrapped” to produce a length-4096 vector of grayscale intensity. 
Labels of either 0 or 1 were used to denote cats from dogs. 

Data Reduction: 
Principal Component Analysis (PCA) was used to reduce the dimensionality of the dataset to 6 set dimensions (10, 25, 50, 100, 250, 500). 

Testing/Training Data:
An 80-20 split was applied to partition images for training and testing data.
5 folds were used to split the data randomly.


Evaluating Classification Techniques: 
For each of the 6 dimensionality reduction parameters, LDA, QDA, and Closest Average Classifiers were applied, and testing/training errors were calculated. 


Visual Creation: 
A line chart was generated to visualize the average testing/training error rates across the set dimensions for each classifier.


![image](https://github.com/justinl138/Pet-Classifier/assets/154792012/6c166d11-024b-4185-8160-189366cda7f7)
