# Spark-EDA-and-model-fitting

Note: This is a capstone project of the datascience nanodegree by Udacity

## Project overview
This is the final project of the datascience nanodegree (DSND). We have an example of a virtual company called 'Sparkify' who offers paid and free listening service, the customers can switch between either service, and they can cancel their subscription at any time. The given customers dataset is huge (12GB), thus the standard tools for analysis and machine learning will not be useful here as it will not fit in the computer's memory (even the data can fit in the memory of a 32GB computer, the analysis, and computations require way more than that amount, and the analysis will crash the system). The safe way to perform such analysis is to do it using Big Data tools like Apache Spark which is one of the fastest big data tools.

For this tutorial, we worked with only a 128MB slice of the original dataset.

The problem is to create a machine learning model to predict the user intent to unsubscribe (Called customers' churn) before this happens.

## Files in this repo


* Sparkify.ipynb: The main coding file in jypyter notebook format to work in Udacity workspace.
* Sparkify.html: an HTML file for the jupyter workbook
* README.md: This file.
* saved_user_dataset_pd.CSV: The extracted dataset for machine learning in csv format


## Used resources
* Python 3.6.x (The programing language)
* pySpark 2.4.x (Machine learning library for big data)
* matplotlib 3.03 (A plotting library)
* pandas 0.23 (numerical calculations library)
* jupyter (The programming notebook interface)


## Summmaries and conclusion
* This capstone project is a great exercise allowing to put in practice several data science skills (data analysis, cleaning, feature extraction, machine learning pipeline creation, model evaluation and fine tuning…) to solve a problem close to those regularly encountered by customer-facing businesses.
* We could get a F1-score of 0.7 for churn prediction using a default classifier algorithm, and 0.73 after fine-tuning; these numbers are relatively good, though not great, maybe because we only have 225 distinct users in our subset.
* This project allowed us to familiarize with Spark; one of the outstanding features of this framework is SQL support, which (even though some limitations exist) is very powerful and enables us to explore data and extract features in a pretty convenient way.
* Next step would be to see how our results extend to the whole dataset (12GB); since all dataset manipulation and machine learning steps were written using Spark framework, we can expect to leverage its distributed cluster-computing capabilities to tackle the big data challenge.

## Potential improvements
* Working with more observations by increasing the dataset size (which is possible in our case by working with the 12GB full dataset)
* Trying more parameters of the selected models.
* Adding some more features that I believe essential, like the customer location (city/state). The customers of some states appear to have more ability to churn than others; this might be attributed to the nature of life there, some lifestyle profiles force people to be rapidly bored, and thus they like to change the services they use, and trying to try other services. On the other hand, peaceful environment make people settled with what they have and resist change.
