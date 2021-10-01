# Agriculture-production
## Data Science Portfolio
Repository Containing portfolio of data science projects completed by me for academic, self-learning and hobby purposes. Presented in the form of ipython notebook and R markdown files. 

Note: Data used in the projects (accessed under data directory) is for demonstration purposes only. 
## __Contents__

-	Overview
-	Motivation
-	Problem statement
-	Goal
-	Install & Import Libraries
-	Data Analysis
-	Feature Engineering
-	Feature Selection
-	Model Building
-	Model Deployment

## __1. Project on Agriculture Production__
## __Overview__
- This project is based on precision farming. In this we will build predictive model with the help of machine learning. This predictive model will help us to understand about which crop is best for soil and climatic conditions. Agriculture is very dependent on soil and climatic conditions. Sometimes climatic condition become unpredictable such as sudden rains, heat waves and fluctuating humidity to cause considerable damage to the farming, due to which the farmer has a lot of problems, he is unable to use his agriculture land well, he cannot use his potential of their land for this we use predictive farming to solve these problems.
Motivation
- What could be a perfect way to utilize unfortunate lockdown period? Like most of you, I spend my time in cooking, Netflix, Coding and reading some latest research papers on weekends. The idea of classifying agriculture production struck to me when I was browsing through some research papers. I couldn’t find any relevant research paper (and of course dataset) associated with it. And that led me to collect the dataset of agriculture production to train a machine learning model using the amazing tools.
Problem statement
- Build a predictive model to suggest the most suitable crops to grow based on the available climatic and soil conditions. 

## __Goal__
Achieve precision farming by optimizing the agriculture production.
Install & Import Libraries
•	Install pandas
•	Install NumPy
•	Install seaborn
•	Install matplotlib
•	Install ipywidgets Then import all the libraries.

## __Date Analysis__
- i.	Read data set
- ii.	Find Missing Values: - Any machine learning model will not work with missing values. First, we find missing values with null function in python. So, in my dataset there is no missing values.
- iii.	Find how many crops are in my dataset by using value count function which says about all unique occurrences of all columns.
- iv.	Now find the average requirements of soil and climatic conditions.
- v.	Now using the @interact function from ipywidgets library to find the maximum, minimum and average requirements for each soil and climatic conditions.
- vi.	Now using the interact function from ipywidgets to find the average soil and climatic requirements for each & every crop.
- vii.	Now we should create a function that let us know which crops have low requirements from the average and which crops have high requirements from the average.
- viii.	Let's check the distributions of all the soil and climatic conditions for all the crops present in this data set.
-	ix.	Now use the filter function of python to find out the name of crops which has unusual requirements.
-	x.	Let's understand which crops can only grow in summer, winter, and rainy season.
## __Model Building__
-	i.	In this I am using clustering analysis. Clustering analysis is a technique that is used to classify data points into relative groups that are called clusters. we can assign similar data points in one group. same as we can build different groups. Infect Clustering analysis is count in unsupervised category that means we can train our model without labels.
-	ii.	from sklearn import KMeans
-	iii.	Now we remove label columns. Now our model is ready for clustering analysis.
-	iv.	Now for performing clustering analysis we must know that how many clusters we required in our dataset so for this we will use Elbow method.
Elbow Method is way from that we can find how many clusters our model required, in this method we will plot no. of clusters with errors and find the Elbow. At which no. we will find the elbow that no. of clusters will be optimum for our model.
-	v.	Plot elbow chart.
- vi.	Now we will implement clustering so in this first we will specify KMeans function and in that we will define compulsory parameter N with the optimal no. of clusters.
- vii.	Now we make predictive model by using machine learning techniques. For this, firstly we must train our dataset.
-	viii.	Predictive Model
Predictive model says about the suitable crops for every specific condition and for making this predictive model we will use machine learning model for train the dataset.
Predictive modeling is also a part of AI. In any predictive model we will make a model by using our dataset and finally when the model will train at that time, we make the predictions for unseen data by using that model.
In the whole process machine learning model will make the decisions rules from the data with the help of every patterns &trends which are very helpful in the final predictions.
- __How can you trust a model that gives us right predictions?__
To check the model performance, we have many different types of evaluation matrixes. With the help of these matrixes, we can find how much accurate is our model and how much trust we can on our model.
Evaluation Matrix: - We use the evaluation matrix to analysis the performance and trust of our model. Evaluation matrix gives us an accuracy score and with the help of that score we can understand how much our model is accurate.
##  Result
So according to classification report our precision values and recall values are very high. So, our model is accurate. To check the results are correct or not. In this case we input values in the model for a particular crop and then check the return output will be that crop or not.

