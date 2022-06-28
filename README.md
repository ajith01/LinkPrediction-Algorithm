# LinkPrediction-Algorithm
Link Prediction Algorithm and Graph Neural Network implemented to make predictions of hidden or future relationships between nodes in a social network. This was a part of my Thesis for undergraduate work. The code was moved to this github as is without any changes made. 

<hr> 

## Set-up 

All these files are set up to run ``google colab``. 

Upon start-up, the program will install all the required modules to the the local enviroment. 

``LinkPredictionNetworkxV2.ipynb`` contains the traditional link prediction algorithms. ``locallyAdaptiveSimilarityMessure()`` is implementation of the classical link prediction algorithm proposed in the paper. It can be used to predict the chance of link forming between any two nodes. 
``computeAUC()`` is used to calculate the AUC score for accuracy of link prediction between randomly chosen nodes. ``compute_AUC_for_no_common_Neighbours()`` does the same, but only for nodes without any common neighbours.  

<br> 

``V2LinkPredictionUsingDeepSnap_v2.ipynb`` contains the graph neural network model for link prediction proposed in my thesis. The dataset required for the introduction is not included. This part can be commented out. The dataset required for training and predicting will be automatically downloaded. This code can support various metrics. The metrics can be chanced by commenting in and out the lines in the ``test()`` functions. 

<br> 

For a <em>very detailed</em> explaination of the algorithm and the GNN model, please look at ``thesis.pdf``. 
