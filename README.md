# Startup Classifier

> Code and academic paper for startup classifier. For Viktor Kozhuharov's internship in Vela Partners, with Yigit Ihlamur as a supervisor.

## Description

A startup classifier that predicts whether a given startup will be successful. Uses two datasets of successful and unsuccessful companies that Vela Partners have provided.

## Methodology

The classifier uses logistic regression. K-nearest neighbours and random forest were also tested but performed worse. The data we use excludes any startups for which we don't have full information. The features *'name'* and *'country_code'* are removed because they are irrelevant (*'country_code'* is always *USA*). *'founded_year'* is also excluded, as it is very hard to extrapolate patterns about specific past years to the current year. A new feature *'number_of_founders'* is added. Other than being able to predict a startup's success, the model also outputs a sorted list of features by their importance.