# Topic-Modelling-NLP-
In this project, I have worked with a dataset of over 400,000 quora questions that have no labeled category, and attempted to find 20 topic categories to assign these questions to. 
I have preprocessed the dataset using TF-IDF Vectorizer.
After converting the data into the format of document-term-matrix , I have implemented Non Negative Matrix Factorization Algorithm (Unsupervised ML Algorithm). I have selected 20 topics to label this dataset of over 400,000 quora questions.
I have used NMF (Non Negative Matrix Factorization) instead of LDA (Latent Dirichlet Allocation) because of large amount of data. 
I have finally added a new column to the original quora dataframe that labels each question into one of the 20 topic categories.   
