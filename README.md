# SVD-Classifier-for-Handwritten-Digits

The 3 main tasks of this project (for a graduate course) are as follows:

1.	Tune the algorithm for accuracy of classification. Give a table or graph of the percentage of correctly classified digits as a function of the number of basis vectors. 
2.	Check if all digits are equally easy or difficult to classify. Also look at some of the difficult ones, and see that in many cases they are very badly written.
3.	Check the singular values of the different classes. Is it motivated to use different numbers of basis vectors for different classes? If so, perform a few experiments to find out if it really pays off to use fewer basis vectors in one or two of the classes

In the sequel, we perform a two-stage classification, in order to save operations in the test phase. In the first stage, we compare the unknown digit only to the first singular vector in each class. If for one class the residual is significantly smaller than for the others, we classify it as that class. Otherwise perform the algorithm descrived above. Fianlly, we report how frequently is the second stage unnecessary.
