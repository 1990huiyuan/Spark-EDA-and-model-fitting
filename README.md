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


## Conclusions
The machine learning modeling succeeded in predicting the customers' activity that will most probably end in unsubscribing. Despite the good results of all the models, the Decision Tree Classifier model appears to be the best here. However, the other models need to be re-adjusted using different settings to reduce the overfitting.

## Potential improvements
* Working with more observations by increasing the dataset size (which is possible in our case by working with the 12GB full dataset)
* Trying more parameters of the selected models.
* Adding some more features that I believe essential, like the customer location (city/state). The customers of some states appear to have more ability to churn than others; this might be attributed to the nature of life there, some lifestyle profiles force people to be rapidly bored, and thus they like to change the services they use, and trying to try other services. On the other hand, peaceful environment make people settled with what they have and resist change.
