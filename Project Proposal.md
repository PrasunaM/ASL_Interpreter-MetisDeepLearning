# Interpreting Sign Language using Neural Networks

### Question/need:
* What is the framing question of your analysis, or the purpose of the model/system you plan to build?

[American Sign Language/ASL](https://www.nidcd.nih.gov/health/american-sign-language) is a primary means of communication for deaf, hard of hearing and hearing nonverbal children who are nonverbal due to conditions such as down syndrome, autism and other speech disorders. Deaf students are considered as a linguistic minority and I'm hoping with this project to promote awareness and acceptance of the language among others. 

Majority of general population is unable to communicate in sign language and the aim of this project is to interprete signs from ASL into English alphabets. 

* Who benefits from exploring this question or building this model/system?

Communication is a key factor for a healthy social life and making tools that can easily translate ASL can help people in need feel included. 

### Data Description:

* What dataset(s) do you plan to use, and how will you obtain the data?

Data is downloaded from [Kaggle](https://www.kaggle.com/datamunge/sign-language-mnist) as a CSV file and consists of image information for each alphabet in sign language except for 9=J or 25=Z because of gesture motions. Train and test files are included seperately. Some image preprocessing was performed according to the data description such as cropping, grayscaling, resizing, addition of filters ('Mitchell', 'Robidoux', 'Catrom', 'Spline', 'Hermite'), with 5% random pixelation, +/- 15% brightness/contrast, and 3 degrees rotation. 

* What is an individual sample/unit of analysis in this project? What characteristics/features do you expect to work with? 

Dataset contains 27000 rows and 785 columns. Columns include label (alphabet the picture belongs to) and pixel (pixel1, pixel2....pixel784) information. All the data is numeric. 

* If modeling, what will you predict as your target?

Using Neural Networks I would to predict to which alphabet the picture belongs to. 

#### Tools:
* How do you intend to meet the tools requirement of the project? 

Keras and other neural network libraries will be used

* Are you planning in advance to need or use additional tools beyond those required?

Google colab if needed to speed up modelling. 

#### MVP Goal:
* What would a [minimum viable product (MVP)](./mvp.md) look like for this project?

MVP will have results from logistic regression as a baseline and a neural network without tuning. 








