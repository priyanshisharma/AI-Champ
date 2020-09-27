## Glossary of terms

* **Online Machine Learning** - It is a method of machine learning in which data becomes available in a sequential order and is used to update the best predictor for future data at each step, 
as opposed to batch learning techniques which generate the best predictor by learning on the entire training data set at once. Online learning is a common technique
used in areas of machine learning where it is computationally infeasible to train over the entire dataset, requiring the need of out-of-core algorithms.
* **Out of Core Learning** - External Memory Algorithms or Out-of-Core algorithms are algorithms that are designed to process data that are too large to fit into 
a computer's main memory at once. Such algorithms must be optimized to efficiently fetch and access data stored in slow bulk memory (auxiliary memory) such as 
hard drives or tape drives, or when memory is on a computer network.
* **Model Based Machine Learning** - ML Algorithms that build models.
* **Validation Set** - Used to calculate accuracy and compare with other models.
* **Train dev set** - The goal of dev-set is to rank the models in term of their accuracy and helps us decide which model to proceed further with. Using Dev set we
rank all our models in terms of their accuracy and pick the best performing model.


## Kaggle
Interesting notebooks for titanic dataset and getting started are:
* https://www.kaggle.com/fermat1/my-first-titanic-notebook-thoughts-from-a-novice
* https://www.kaggle.com/alexisbcook/titanic-tutorial

## Doubts
* In the quiz, spam detection was supposed to be classified as *Supervised* or *Unsupervised*, but couldn't is be both? Anomaly detection for unsupervised and 
classification for supervised?<br/>

Spam Detection is **supervised** because there is a possiblity (in the case of multiple subscriptions) that spam emails are more frequent or nearly as frequent as regular emails, thereby they aren't anomalies. (Anomalies <<< Normal)

* Running the following in python: 
```
a = np.arange(14)
c = np.array(range(14))
print(a is c)
```
even though they look exactly same on printing `a` and `c`, the condition `a is c` is `False`. Why?<br/>

Their values are same, they aren't.

* Is *validation* set and *cross-validation* set different?<br/>
Yes they're different. Cross - Validation comes up in situations like k-fold cross validation. Look at the illustration below. <br/>
![Cross Validation](cross-validation.png)

* Difference between *Train dev set* and *validation set*? (As I happen to believe they both are for comparing algorithms.) <br/>
They're the same.
