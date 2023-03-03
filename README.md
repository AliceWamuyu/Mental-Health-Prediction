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
Despite resources in Kenyan universities growing immensely over the years, development of support services to students has not.Research has shown high levels of mental health problems among university students specifically depression and anxiety with the most affected group being students from poor backgrounds. The lack of or little provision for support services for such students results in dropouts and their inability to reach their full potential. 
The use of technologies including machine learning and AI will potentially transform the delivery of mental health services in the coming years.This challenge aims to develop a machine learning model that classifies statements and questions expressed by university students in Kenya when speaking about the mental health challenges they struggle with and come up with a chatbot that will be used for a prototype of a mental health chatbot designed specifically for university students. 

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

## Conclusion
***

## Limitations
***

## For More Information
***
See the full analysis in the [Jupyter Notebook](https://github.com/FridahKimathi/Water-Pump-Functionality-Prediction-in-Tanzania/blob/main/index.ipynb) or review this [presentation](https://github.com/FridahKimathi/Water-Pump-Functionality-Prediction-in-Tanzania/blob/main/Water%20Pump%20Functionality%20Prediction%20PPT.pdf).

## Repository Structure
***

```
├── Data
├── Images
├── README.md
├── Water Pump Functionality Prediction PPT
└── index.ipynb
```