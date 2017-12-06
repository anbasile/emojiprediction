# emojiprediction

Code for the 2018 SemEval Emoji Prediction task

## Baselines

### EN
Using the SVM

    pipe = Pipeline([('tfidf', TfidfVectorizer()),
	                 ('clf', LinearSVC())])
    cross_val_score(pipe, X_us, Y_us, cv=5)
    array([ 0.33393839,  0.33468285,  0.33348292,  0.33618228,  0.33255477])
	
Using Naive-Bayes	

    pipe = Pipeline([('tfidf', TfidfVectorizer()),
                     ('clf', MultinomialNB())])
    cross_val_score(pipe, X_us, Y_us, cv=5)
    array([ 0.24824857,  0.24882725,  0.24888322,  0.24944925,  0.24829668])

### ES

Using the SVM
 
Using Naive-Bayes	

	pipe = Pipeline([('tfidf', TfidfVectorizer()),
                 ('clf', MultinomialNB())])
	cross_val_score(pipe, esp_text, esp_labels, cv=5)
	array([ 0.21672407,  0.21726356,  0.21785389,  0.21898439,  0.21963706])





