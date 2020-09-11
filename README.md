# Simulation-of-Selective-Bayesian-Classifier-

This is review and simulations of paper "Scaling up the Naive Bayesian Classifier: Using Decision Trees for Feature Selection" by Ratanamahatana & Gunopulos(2002) using R and ecoli dataset.  

MOTIVATION: 
It is proved that enhancement and optimization of Naïve Bayes(NB) has always been a challenging task. Most of the research done have tried boosting of NB where multiple classifiers are  used to obtain the misclassification rate, but these approaches are not applicable to all the domains. Another approach was to use only those features that are more relevant. These attributes are found as a result of applying decision tree and KNN, though decision trees are immune to correlated features but if the training set is large enough the tree becomes too complex. The motive of selecting this paper with respect to others is that it takes up on different approach to optimize NB called Selective Bayesian Classifier (SBC) here they have particularly concentrated on feature subset selection where C4.5 decision tree is used to obtain the subset of features and NB is trained and tested with only these features. If only relevant and highly optimal features are used NB is proven to show better results, also complexity of the model is reduced, and the model learns faster than NB model without feature selection. 

SELECTIVE BAYESIAN CLASSIFIER 
 The main aim of this paper is to enhance the NB classifier by subset optimal features from the set and to remove highly correlated features. SBC is developed by combination of C4.5 and NB. It is known that NB works on a conditional independence assumption and C4.5 constructs its tree considering features that are most relevant. The reason for choosing C4.5 for feature selection in SBC is that C4.5 constructs simple tree if there are smaller number of training set and when training set increases the features are selected such a way that they are not correlated because C4.5 considers only one set of correlated feature set to make split. If the tree becomes too complex i.e. if there are many branches, then SBC is structured such a way that it only selects the features from first three levels of the tree. This method of feature selection helps us to improve the performance of NB classifier without having to compromise the accuracy. The SBC algorithm works as follows (Ratanamahatana & Gunopulos, 2002).

REFERENCES
[1]	Ratanamahatana, C. “Ann,” & Gunopulos, D. (2002). Scaling up the Naive Bayesian Classifier: Using Decision Trees for Feature Selection. Retrieved from https://www.semanticscholar.org/paper/Scaling-up-the-Naive-Bayesian-Classifier-%3A-Using-Ratanamahatana-Gunopulos/bee1fb17a8c6610f46ec10fe3f8cf67f5242eaa6

[2]	Awati, K. (2015). A gentle introduction to Naïve Bayes classification using R. A Gentle Introduction to Naïve Bayes Classification Using R. Retrieved from https://eight2late.wordpress.com/2015/11/06/a-gentle-introduction-to-naive-bayes-classification-using-r/ 

[3]	Hornik, K. (2020). An R interface to Weka (Version 3.9.3). Retrieved from https://cran.r-project.org/web/packages/RWeka/RWeka.pdf 

[4]	Hothorn, T., & Zeileis, A. (2020). A Toolkit for Recursive         Partytioning. Retrieved from https://cran.r-project.org/web/packages/partykit/partykit.pdf 

[5]	Zeileis, A. (2015). Properties and their values out of J48 tree (RWeka). Retrieved from https://stackoverflow.com/questions/32168408/properties-and-their-values-out-of-j48-tree-rweka 

[6]	 Lateef, Z. (2019, May 22). A Comprehensive Guide To Naive Bayes In R. Retrieved from https://www.edureka.co/blog/naive-bayes-in-r/ 

[7]	Saha, S. (2018, August 20). What is the C4.5 algorithm and how does it work? Retrieved from https://towardsdatascience.com/what-is-the-c4-5-algorithm-and-how-does-it-work-2b971a9e7db0 

