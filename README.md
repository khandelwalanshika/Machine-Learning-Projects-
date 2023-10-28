# Topic-Modelling-NLP-
In this project, I have worked with a dataset of over 400,000 quora questions that have no labeled category, and attempted to find 20 topic categories to assign these questions to. 

Imported utilities, libraries and important packages used throughout : sklearn, pandas, numpy.

We import the quora dataset consisting of features: "Question" : 400,000  quora questions.

Subsequently, in the Preprocessing step, we use TF-IDF Vectorizer as a feature extraction technique and transform the "Question" feature to a vectorized document term matrix. We use (max_df) and (min_df) parameters to remove the words occurring across 95 % of the documents and the minimum occurring words across 2% of the documents along with stop words. 

After converting the data into the document-term-matrix , I have implemented Non Negative Matrix Factorization Algorithm (Unsupervised ML Algorithm). I have selected 20 topics to label this dataset of over 400,000 quora questions by setting (n_components=20) and selecting random_state as 42 during the implementation of the model.

Non negative matrix Factorization Algorithm factorizes the original document term matrix into a product of matrix of base vectors  or feature matrix and a coefficient matrix. 
It wirks according to the principles of dimentionality reduction and feature extraction. 

The assumption of this algorithm is that the original matrix is composed of hidden feature matrix W and weights matrix H respectively. 

I have used NMF (Non Negative Matrix Factorization) instead of LDA (Latent Dirichlet Allocation) because of large amount of data. LDA is a probabilistic model, whereas NMF is a Linear Algaebraic model.

I have finally added a new column to the original quora dataframe that labels each question into one of the 20 topic categories.   
