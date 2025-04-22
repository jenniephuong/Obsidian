> profile based, specialised intelligent analysis of security events through statistics, machine learning and artificial intelligence that compares current activity (traffic) with stored profiles (baselines) of normal activity so anything not normal is a candidate for analysis.

what are pros of anomaly based
- many tools are open source 
- more adaptable, and can learn to detect 'unknowns' through patterns

what are the cons of anomaly based 
- requires specific skills like programming and maths
- limited generalisability - need to define what 'normal' is, however 'normal' can be dynamic and constantly changing e.g. out of hours upgrades or early workers will spike traffic in abnormal times

how does anomaly detection work
1. identify distinct **[[Feature Selection|features]]**
    - each column or variable in a dataset is a feature
2. establish a **baseline** normality
    - density plot, histogram
3. monitor **deviations** from the baseline as an anomaly
    - skew, major outliers, identify distinct features

![[Pasted image 20250422102102.png]]


what approaches can be used for anomaly detection
- statistical - looking for correlations and significant deviations from the normal data
- ![[Pasted image 20250422102722.png|300]]
- supervised - used a known dataset to build a 'normal' model and make predictions for future data points
- ![[Pasted image 20250422102754.png|300]]
- unsupervised - infer relationships by grouping points in unlabelled data
- ![[Pasted image 20250422102837.png|300]]


what are examples of statistical approaches 
- frequency analysis - with the distinctive features of number of connections by time ![[Pasted image 20250422102624.png]]
- chi-squared
- pearson's correlation
- t-test
- ANOVA
- kruskal-wallis
- principle component analysis 


what are examples of supervised approaches
- decision trees 
- neural networks 
- bayesian networks
- support vector machines 
- regression

what are examples of unsupervised approaches
- hierarchical clustering
- k-means clustering
- self organising maps
- hidden markov models

