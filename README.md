# **Mental Health Prediction for Kenyan university students**

<img src="Images\mental-health-episode-page.jpg" alt="Mental Health image" width="750" height="400">

#### **Authors**: 
[Alice Wamuyu](alice.wamuyu@student.moringaschool.com),
[Eugene Kuloba](eugene.kuloba@student.moringaschool.com),
[Fridah Kimathi](mailto:fridahnkirotekimathi@gmail.com),
[Karen Amanya](karen.amanya@student.moringaschool.com),
[Nicholus Magak](nicholus.magak@student.moringaschool.com) and
[Nobert Akwir](nobert.akwir@student.moringaschool.com).

## Overview
****
The project aims to create a machine learning model that can classify statements and questions related to mental health challenges expressed by university students in Kenya. 

## Business Problem
***
<p>Despite resources in Kenyan universities growing immensely over the years, development of support services to students has not.Research has shown high levels of mental health problems among university students specifically depression and anxiety with the most affected group being students from poor backgrounds. The lack of or little provision for support services for such students results in dropouts and their inability to reach their full potential. </p>
<p>The Africa Mental Health Foundation is an NGO that aims at conducting mental health research to get findings that aid in developing innovative practices for providing mental health services in Africa. In 2023, they are partnering with the ministry of Education in Kenya to develop a chatbot that will be available to all university students in Kenya. The goal of this is to  reduce the stigma around seeking help by providing the students with a platform where they can openly input their feelings / thoughts and this will attempt to classify the particular problem they are facing and therefore provide fitting resources.</p>
<p>This project aims to develop a machine learning model that classifies statements and questions expressed by university students in Kenya when speaking about the mental health challenges they struggle with and come up with a chatbot that will be used for a prototype of a mental health chatbot designed specifically for university students. </p>

## Data
***
The data used in this project is from the <a href="https://zindi.africa/competitions/basic-needs-basic-rights-kenya-tech4mentalhealth/data">Basic Needs Basic Rights Kenya - Tech4MentalHealth</a> competition hosted by <a href="https://zindi.africa/"> Zindi Africa</a>. The data consists of statements and questions expressed by students from multiple universities across Kenya who reported suffering from these different mental health challenges. The wording of the statements is intended to respond to the prompting question, “What is on your mind?”

## Modelling
***
Different models were evaluated and the best performing model was picked to be the final model.The XGBoost Classifier was picked as the final model, with its parameters being the best parameters found through grid search.

                 Models
<img src="Images\models.jpg"  width="650" height="400"> 

## Evaluation
***
<p>Based on the accuracy of our best model, the XGBoost Classifier-Grid Search, had a train accuracy score of 92% and test accuracy of 85%. The same model had a train and test log score of 0.242 and 0.439, respectively. We chose to use log loss as a performance metric because it takes into account the probabilities underlying in the model, not only the final output of the classification. This means, the higher the probabilities the lower the log loss value, which is better because it is basically a measure of uncertainty and the lower it is, the more certain we are of the potential occurrence. </p>
<p>Since XGBoost classifier had the lowest log loss score, and it was chosen to be the best model, even though we had prior models with high training and test data accuracy.</p>

## Limitations
***
<ul>
<li>Due to the imbalance in the dataset the F1-score for drug and alcohol was notably lower than depression and suicide.</li> </br>
<li>Due to a relatively small dataset we could not achieve high score as desired.</li> 
</ul>

## Conclusion
***
The final model performed fairly well with a log score of 0.52 and an accuracy of around 85%. The Africa Mental Health Foundation(AMHF) can integrate the model into a chatbot prototype to carry out tests on actual university students and predict the student's mental state in order to assist them accordingly. This will help correctly identify and classify mental health problems to match students with the suitable resources. Moreover, the developed chatbot will encourage more students to  openly seek help without the fear of stigmatization.

## Recommendations
***
<ul>
<li>The Africa Mental Health Foundation(AMHF) should collect more data that features drug and alcohol related problems as well as other mental health problems that have not been featured in the observations used here.</li> </br>
<li>The model be integrated into the chatbot prototype to carry out tests on actual university students and collect data on how it performed in classifying problems they were facing.</li> </br>
<li>The chatbot should also feature a database containing resources and services available to the students based on the problem that the model was able to identify. This will ensure that actual help is availed to the user.</li>
</ul>

## For More Information
***
See the full analysis in the [Jupyter Notebook](https://github.com/AliceWamuyu/Mental-Health-Prediction/blob/main/index.ipynb) or review this [presentation](https://github.com/AliceWamuyu/Mental-Health-Prediction/tree/main/Presentation).

## Repository Structure
***

```
├── Data
├── Images
├── README.md
├── Mental Health Prediction - PPT.pdf
└── index.ipynb
```