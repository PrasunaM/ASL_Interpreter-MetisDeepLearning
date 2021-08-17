# Interpreting Sign Language using Neural Networks

[American Sign Language/ASL](https://www.nidcd.nih.gov/health/american-sign-language) is a primary means of communication for deaf, hard of hearing and hearing nonverbal children who are nonverbal due to conditions such as down syndrome, autism and other speech disorders. Currently, there is a shortage of interpreters in the US and the U.S. Bureau of Labor Statistics estimates a rise of 19% ASL interpreter by 2028.

The aim of this project was to interprete signs from hand images of ASL into English alphabets using neural networks. Data is downloaded from [Kaggle](https://www.kaggle.com/datamunge/sign-language-mnist) as a CSV file and consists of image information for each alphabet 

An accuracy of 0.97 was obtained using convolutional neural network was obtained. Transfer learning was attempted which could not outperform CNN. 

# Workflow

1. [EDA & Logistic Regression](Final_submission/1)
2. [Convolution Neural Network](Final_submission/2) 
3. [Attempt with Transfer Learning](Final_submission/3) 
4. [Presentation Slides](Final_submission/DeepLearningSlides.pdf)

# Conclusion

Best accuracy was obtained using CNN with 5 conv2D layers and 3 dense layers. Overfitting was addressed with drop out, batch normalization and early stopping. 
Attempt for a better accuracy will be made in the future with more image data. 








