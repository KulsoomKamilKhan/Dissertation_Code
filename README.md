# Predicting Money Laundering Transactions using Machine Learning
This project compares 6 machine learning models (RF, LR, SVM, KNN, LOF, CBLOF) and 2 Deep Learning models (RNN-LSTM, Autoencoders) on two distinct financial datasets. 

The datasets selected were publicly available and anonymised:
- Elliptic Bitcoin Dataset - real-world dataset
- IBM AMLSim Dataset - synthetically generated dataset

Following tables charts the model comparison for each dataset:
![image](https://github.com/KulsoomKamilKhan/Fraud_Detection_ML/assets/71809252/027bc9c2-7df2-4014-850b-030f19eb85d0)
![image](https://github.com/KulsoomKamilKhan/Fraud_Detection_ML/assets/71809252/6a521a5b-e475-499b-b4b5-3c6dca5f3b4f)

### Observations:
Through the observations made in the above tables, we can conclude that supervised models work best for both datasets. But this performance scoring is not enough. Rarely in real-life do we find financial transactions labelled. Scarcity of labels would render the supervised models performance void. Similarly, Unsupervised models do not generally perform well in detecting outliers in fraud data as they can be present in the majority class. In such cases, semi-supervised models should be used, as done in the case of Autoencoders. This proved to be our best working example as shown for the AMLSim dataset, which is a synthetic dataset, and comes close to the supervised RF model baseline score for the Elliptic Bitcoin datset.

The difference in performance can also be due to the structure of both datsets, as normal financial transactions are different from Bitcoin Blockchain transactions. Models need to be developed to suit their dataset values accordingly, but we can conclude through the experiments done on this project, that semi-supervised models managed to bring the most information out of each of the datasets, and helped classify the samples best.

### How to run the notebooks:
Please download all the imports and dependancies present in both the Elliptic Dataset and AML SIM dataset notebooks before running them. The datasets associated with each notebook can be found at the following link:  
https://heriotwatt-my.sharepoint.com/:f:/r/personal/kkk6_hw_ac_uk/Documents/Dissertation%20Datasets?csf=1&web=1&e=5S9RD3
