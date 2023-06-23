# NeuralNet-In-MSFT-Excel-Visual-Learning-Tool
To help people and myself learn how neural networks and machine learning work I decided to start working on an excel representation of a simple neural network.  

Lambda Functions to Represent Softmax Activation Functions in Excel

#excel/neural_net_model #machinelearning


## After setting up LAMBDA functions

Ok all setup and working great. lets do a test. so i created the first two LAMBDA functions and created two simple test variables to hold the input values, x = .5, and array = [1, 0.5, 0.3]. i think passed both of these functions to the last function / step you provided which combines the first 2 help calculation functions, or =LAMBDA(x,array, EXP(x)/SUMPRODUCT(EXP(array))) and the output was exactly one scalar value of 0.29. 


## Verify your Lambda function result. Given x = 0.5 and the array = [1, 0.5, 0.3], applying the softmax function to x, we have:

- First, we calculate the exponent of each value in the array: `e^1`, `e^0.5`, `e^0.3` which are approximately [2.718, 1.649, 1.350].
- Then, we sum up these values: 2.718 + 1.649 + 1.350 = 5.717.
- Finally, we calculate the softmax of x = 0.5, which is `e^0.5 / 5.717` = 1.649 / 5.717 = ~0.288.

So your Excel setup seems to be correct! Your calculation returned 0.29 which is close to my manual calculation of 0.288, the difference might be due to the precision of the calculations.

Now, for the glossary and the symbols, here are some common terms and symbols used in linear algebra and matrix calculus:

- Matrix: A rectangular arrangement of numbers into rows and columns, typically represented by bold uppercase letters, e.g., **A**, **B**.
    
- Vector: A matrix with just one row or one column, typically represented by bold lowercase letters, e.g., **a**, **b**.
    
- Scalar: A single number, typically represented by lowercase italic letters, e.g., a, b.
    
- Addition of matrices: Two matrices can be added if they have the same dimensions, by adding the corresponding elements. Symbol: **A** + **B**
    
- Subtraction of matrices: Two matrices can be subtracted if they have the same dimensions, by subtracting the corresponding elements. Symbol: **A** - **B**
    
- Multiplication of matrices: Two matrices can be multiplied if the number of columns in the first matrix is equal to the number of rows in the second matrix. Symbol: **A** * **B**
    
- Division of matrices: Division is not directly defined for matrices. However, you can multiply by the inverse of a matrix. Symbol: **A** * **B**^-1
    

As for your question about row vectors and column vectors, in strict mathematical terms, they are not exactly the same. A row vector is a single row matrix, and a column vector is a single column matrix. In many contexts, however, we can freely transpose between the two (i.e., turn a row vector into a column vector and vice versa) without changing the underlying data they represent. But it's important to be aware of what form your vector should be in for specific mathematical operations.
