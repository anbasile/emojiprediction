# emojiprediction

Code for the 2018 SemEval Emoji Prediction task

## Baselines

Using the SVM

    pipe = Pipeline([('tfidf', TfidfVectorizer()),
	                 ('clf', LinearSVC())])
​
    cross_val_score(pipe, X_us, Y_us, cv=5)

    array([ 0.33393839,  0.33468285,  0.33348292,  0.33618228,  0.33255477])
	
Using Naive-Bayes	

    pipe = Pipeline([('tfidf', TfidfVectorizer()),
                     ('clf', MultinomialNB())])
​
    cross_val_score(pipe, X_us, Y_us, cv=5)

    array([ 0.24824857,  0.24882725,  0.24888322,  0.24944925,  0.24829668])
