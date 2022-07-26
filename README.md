# FakeNewsPredictor
When any news are spread across internet we don't know whether it's real news or fake news. So to solve this problem I used Passive Aggressive Classifier algorithm to train this model and deployed it with the help of docker on heroku platform.

## Steps involved in this project
### step 1: Data collection
Collected dataset from Kaggle to train the model and handling some missing values.
link : https://www.kaggle.com/c/fake-news/data?select=train.csv
### step 2: Data preprocessing
we can't directly take the dataset and train our model. Because those data are represent in textual form, we need to convert it into the numerical form. Here we use TfidfVectorizer for conversion.
### step 3: Train the model and check the accuracy
For better accuracy we go for PassiveAgressiveClassifier model for this problem and it gives almost 99% accuracy rate.
### step 4: Deploy the model with the help of docker on heroku platform
To create a CI/CD pipline we use Docker. I created a flask app and wrap it into the Docker container and with the help of github actions I deployed it on heroku as container.
