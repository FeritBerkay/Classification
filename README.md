# Classification

In this model, I analyzed individual data to classify whether they have diabetes or not, leveraging seven different variables. Initially, I examined the data, checked for null values and duplicates, and then prepared it for the model. Following data preparation, I proceeded to scale and split it. Subsequently, I applied three classifiers: Logistic Regression, SGDClassifier, and SGDOneClassSvm; and  I assessed the model's performance using metrics such as accuarcy score and classification report. I used SGDClassifier and SGDOneClassSvm models, in order to, utilize gradient descent in the classification model.

While Logistic Regression and SGDClassifier exhibited good accuracy scores, SGDOneClassSvm performed poorly in terms of accuracy. Upon further investigation, I discovered that SGDOneClassSvm is primarily suited for unsupervised tasks. Attempting to use ElasticNetCv resulted in an error due to employing a classification metric in a regression model, rendering the output meaningless.

Ultimately, I achieved the highest accuracy score by running the Logistic Regression model with both L2 (Ridge) and L1 (Lasso) regularization techniques. This approach yielded the best accuracy score using L2 (Ridge) regularization. Consequently, I concluded that, in this context, Logistic Regression with L2 (Ridge) regulaziation exhibited superior performance over other models.

**The dataset originates from the National Institute of Diabetes and Digestive and Kidney Diseases, aiming to predict, based on diagnostic measurements, whether a patient has diabetes.**


#PCA

I examined a genetic dataset containing about 100 genes, each with approximately 10 unique traits. Using Principal Component Analysis (PCA), I identified the main traits that significantly influenced how these genes were grouped together. I then created a program to find the top 10 traits that had the biggest impact on the initial gene groupings, specifically focusing on PC1.








This dataset is originally from the National Institute of Diabetes and Digestive and Kidney Diseases. The objective is to predict based on diagnostic measurements whether a patient has diabetes.
