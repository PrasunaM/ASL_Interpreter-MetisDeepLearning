## ASL Image Interpreter

The goal of this project is classify images of hands interpreting english alphabets. Dataset contains about 20,000 images with 784 columns containing pixel data and label information. A multiclass logistic regression was performed and used as a baseline, CNN and CNN with transfer learning were performed consequently. 

### Logistic Regression 

Logistic Regression performed reasonably well, with an accuracy score of 0.70. Here's the confusion matrix -

<img src="Screen Shot 2021-07-06 at 2.37.44 PM.png" alt="Logistic Regression" width="800" height = "500"/> 

The most common misclassified classes are the letters K and R. 


<img src="Screen Shot 2021-07-06 at 2.17.43 PM.png" alt="K" width="200" height = "200"/>     <img src="Screen Shot 2021-07-06 at 2.17.51 PM.png" alt="R" width="200" height = "200"/> 

### CNN

Data was reshaped to fit a CNN. Initial CNN performed well on train/val with 0.99 accuracy and 0.86 on test data. A drop out of 0.20 for each layer, batch normalization for alternate layers was added to reduce overfitting. Accuracy improved to 0.95. Finally, additional dense layer with 100 units was also added improving accuracy to 0.96. 
Here's the confusion matrix - 

<img src="Screen Shot 2021-07-06 at 2.24.05 PM.png" alt="Logistic Regression" width="800" height = "500"/> 

### CNN with transfer learning

CNN with transfer learning, using weights from imagenet is unfortunately underperforming with an accuracy of 0.80. I will be working improving this model further. 
