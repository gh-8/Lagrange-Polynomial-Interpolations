Lagragne Interpolation Application: Estimating the population of British Columbia
===============

Objective
----------
Construct a fourth degree Lagrange interpolating polynomial to estimate the population of British Columbia Canada. Five given data points are provided from roughly 2011 to 2015. 

Algorithm
-----
Included years 2011 to 2015 as constants along with thier respective population numbers.
Constructed a loop for 10 Iterations (10 years) for implementing the lagrange polynomial:

p_vector(i) = fx1*((x-x2)*(x-x3)*(x-x4)*(x-x5))/((x1-x2)*(x1-x3)*(x1-x4)*(x1-x5)) + fx2*((x-x1)*(x-x3)*(x-x4)*(x-x5))/((x2-x1)*(x2-x3)*(x2-x4)*(x2-x5))+ fx3*((x-x1)*(x-x2)*(x-x4)*(x-x5))/((x3-x1)*(x3-x2)*(x3-x4)*(x3-x5))+fx4*((x-x1)*(x-x2)*(x-x3)*(x-x5))/((x4-x1)*(x4-x2)*(x4-x3)*(x4-x5))+fx5*((x-x1)*(x-x2)*(x-x3)*(x-x4))/((x5-x1)*(x5-x2)*(x5-x3)*(x5-x4))

Results & Observations
-----
After running the MATLAB code, it appeares that the resulting plot of the Lagrange interpolant each ‘x’ on the plot above agrees with the given data from 2011 to 2015. Then the approximation for the the population of BC falls sharply compared to expected.

Other observations: The accuracy of each approximation depends heavily on preceding data points. Small intervals between points seems to help bound error size. Howerver, the further from provided data, the bigger the error size. In fact, there is a large drop from the estimate beginning in 2016. 
