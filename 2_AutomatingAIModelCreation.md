# Automating AI Model Creation with Azure Machine Learning

## Training a Model
- Feed lots of real world data into a program and the program tries to make generalizations about the data. It then uses these generalizations to make predictions when it's given new data. Example: email that is spam or not spam and then organizes once it learns one from the other.

- Course demo:
    - Use ML to predict bicycle rentals on a given day.
    - Feed historical bike rental information into an ML algorithm and get it to generalize about how various factors affect the number of rentals.
    - Use the automated ML features of Azure ML to try different algorithms and see which one works best for bike rental predictions.

- Job vs. Experiment - job is one training run, experiment contains jobs. Usually run multiple jobs to see which model works the best.

- Classification - used when needed to classify data into two or more categories (e.g., animals, speech recognition, sentiment analysis). Supervised learning.
- Regression - used when you need to predict a number (e.g., estimated home selling price based on sales prices of other homes in the past). Needed for including multiple factors (e.g, home age, distance to school) which makes a multi-dimensional graph that is hard to visualize. Supervised learning.
- Clustering - not available in Azure ML learning tool at the moment. Clustering is a type of unsupervised learning. 

- Supervised learning - consists of labeled data. Each piece of training data has a label with an answer. 
- Unsupervised learning - data is unlabeled. Algorithm looks for patterns and tries to group the data into different clusters (e.g., segmentation by purchase history).

## Deploying a Model
- [Training and Deploying a model](https://github.com/cloudacademy/azure-automl).