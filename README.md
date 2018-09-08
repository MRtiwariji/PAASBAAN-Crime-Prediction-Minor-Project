# PAASBAAN-Crime-Prediction-Minor-Project


# Abstract
To be better prepared to respond to criminal activity, it is important to understand patterns in crime. In our project, we analyze crime data from the city of Indore, scraped from publicly available website of Indore Police.
At the outset, the task is to predict which category of crime is most likely to occur given a time and place in Indore.
We also attempt to make our classification task more meaningful by merging multiple classes into larger classes. Finally, we report and reflect on our results with different classifiers, and dwell on avenues for future work.

# Implementation
The implementation of the project is done with the help of python language. To be particular, for the purpose of machine learning Anaconda is being used.
Anaconda is one of several Python distributions. Anaconda is a new distribution of the Python. It was formerly known as Continuum Analytics. Anaconda has more than 100 new packages. Anaconda is used for scientific computing, data science, statistical analysis, and machine learning.
On Python technology, we found out Anaconda to be easier. Since it helps with the following problems:
•	Installing Python on multiple platforms.
•	Separating out different environments.
•	Dealing with not having correct privileges.
•	Getting up and running with specific packages and libraries.
This data was scraped from the publically available data from Indore police website which had been made by people in police station of different areas. Implementation of the idea started from the Indore city itself so as to limit an area for the prediction and making it less complex. The data taken from all the FIR’s was sorted and converted into a new format of timestamp, longitude, latitude, which was the input that machine would be taking so as to predict the crime rate in particular location or city.
The entries was done just to make the machine learn what all it has to do with the data and what actually the output is being demanded. As soon as the machine learnt the algorithms and the process, accuracy of different algorithms were measured & the algorithm with the most accuracy is used for the prediction kernel i.e. Random forest.
# Implementation Details 
For the purpose of proper implementation and functioning several Algorithms and techniques were used. Following are the algorithms used:
# KNN (K-Nearest neighbors)
A powerful classification algorithm used in pattern recognition K nearest neighbors stores all available cases and classifies new cases based on a similarity measure (e.g. distance function).One of the top data mining algorithms used today. A non-parametric lazy learning algorithm (An Instance based Learning method).
KNN: Classification Approach
•	An object (a new instance) is classified by a majority votes for its neighbor classes. 
•	The object is assigned to the most common class amongst its K nearest neighbors.(measured by distance function) 

 
            Fig 4.1.1 Principle diagram of KNN
 
Fig 4.1.2 Shows graphical representation of KNN

 
Fig 4.1.3 Distance functions
# Decision Tree
As the name says all about it, it is a tree which helps us by assisting us in decision-making. Used for both classification and regression, it is a very basic and important predictive learning algorithm.
•	It is different from others because it works intuitively i.e., taking decisions one-by-one.
•	Non-parametric: Fast and efficient.
It consists of nodes which have parent-child relationships:
 
Fig 4.2.2 Decision tree

 
Fig 4.2.2 example

Decision tree considers the most important variable using some fancy criterion and splits dataset based on it. It is done to reach a stage where we have homogenous subsets that are giving predictions with utmost surety.
# Random forest
Random Forests is a very popular ensemble learning method which builds a number of classiﬁers on the training data and combines all their outputs to make the best predictions on the test data.
Thus, the Random Forests algorithm is a variance minimizing algorithm that uses randomness when making split decision to help avoid overﬁtting on the training data.
A random forests classiﬁer is an ensemble classiﬁer, which aggregates a family of classiﬁers h(x|θ1),h(x|θ2),..h(x|θk). Each member of the family, h(x|θ), is a classiﬁcation tree and k is the number of trees chosen from a model random vector.
Also, each θk is a randomly chosen parameter vector. If D(x,y) denotes the training dataset, each classiﬁcation tree in the ensemble is built using a different subset Dθk(x,y) ⊂ D(x,y) of the training dataset.
 Thus, h(x|θk) is the kth classiﬁcation tree which uses a subset of features xθk ⊂ x to build a classiﬁcation model. Each tree then works like regular decision trees: it partitions the data based on the value of a particular feature (which is selected randomly from the subset), until the data is fully partitioned, or the maximum allowed depth is reached. The ﬁnal output y is obtained by aggregating the results thus:
 
where I denotes the indicator function.
 Fig 4.3.1 Example






 
Fig 4.3.2 Random Forest of Paasbaan
# Testing 
The development of software involves a series of production activities were opportunities for injection of human fallibilities are enormous. Error may begin to occur at very inspection of the process where the objective may be enormously or imperfectly specified as well as in lateral design and development stage. Because of human inability to perform and communicate with perfection, software development quality assurance activities.
Software testing is a crucial element of software quality assurances and represents ultimate review of specification, design and coding.   
# White box testing
It focuses on the program control structure. Here all statement in the project have been executed at least once during testing and all logical condition have been exercised. 
# Black box testing
This is designed to uncover the error in functional requirements without regard to the internal working of the project. This testing focuses on the information domain of the project , deriving test case by partitioning the input and output domain of programming – A manner that provides through test coverage.

Test Case ID	Test Name	Test Description	Steps	Executed result	Actual result	Test case statement
01	Check for correct entered numeric values and date and time.	The entered values are in correct format.	1. Enter details in fields.
 2. Click submit.	If format is correct details are sent to kernel successfully.	As expected.	Pass
02	Predicted Result	Output is displayed	If kernel predicts successfully output is then showed to the screen 2.	As expected	Pass
03	Analysis Button	Data visualization is displayed.	1.Click Analysis	Shows the overall analysis on screen 3	As expected	pass





