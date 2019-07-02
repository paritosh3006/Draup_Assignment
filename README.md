# Draup_Assignment
News Classification
The Task

Large volumes of news articles are received every day from various sources. To simplify downstream processing tasks, one of the first steps is to properly categories news into well-defined categories. In this problem, you have been given a set of news articles and a set of categories. Your task is to develop a model which will be able to predict the category of unseen news.

Approach:
1.	Firstly I have imported 1. news_details.xlsx, 2. category_mapping.xlsx, 3.categories.csv and stored them in df1, df2, test_df. After that renaming column 'id' of df3 to category_id to join it with df2 then Join df1 and mapped_data on 'news_id', drop the duplicate rows & reset index.
2.	After that I analyzed the data and checked whether there is a need to remove stopwords  and Lemmatization and then Convert the post corpus to dataframe and Concat the catogories of final_data with data and Transform the string values of category to respective label encoded numeric values..
3.	Now before spliting the dataset  Intiatise TD-IDF Vectorizer and transform the input text data Now fit the model on our training dataset after tuning our hyperparameters using gridsearchcv and predict on our validation set and find the accuracy for the same. I have performed the above process for three classifiers 1. Random Forest  2. MultinomialNB  and 3. Logistic Regression and observed that we are getting more accuracy for Logistic Regression. And then I got the maximum accuracy from Logistic regression
