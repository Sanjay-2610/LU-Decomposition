# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### (i)
1. Importing numpy and lu from scipy.linalg
2. Getting a input for the matrix as array
3. Using the lu function getting the L , U , P matrix for the orginal matrix
4. printing the L and U matrices

### (ii)
1. Importing numpy ,lu_factor and lu_solve from scipy.linalg
2. Getting the matrices A and B as array
3. Using the function lu_factor() getting the lu and piv matrix
4. Using the fuction lu_solve() solving the matrix using the lu,piv as A and B 
5. Printing the Solution
## Program:
(i) To find the L and U matrix
```py
#Program to find L and U matrix using LU decomposition.
#Developed by: Sanjay Ragavendar.M.K
#RegisterNumber: 22009286 

import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U= lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```py
#Program to find the LU Decomposition of a matrix.
#Developed by: Sanjay Ragavendar M K
#RegisterNumber: 22009286

import numpy as np
from scipy.linalg import lu_factor, lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,piv = lu_factor(A)
x= lu_solve((lu,piv),B)
print(x)
```

## Output:
### (i)
![image](https://user-images.githubusercontent.com/91368803/214780072-0a80d11b-1708-456f-9409-207f8c41e811.png)

### (ii)
![image](https://user-images.githubusercontent.com/91368803/214779945-b32b2afe-8f23-4411-ab1a-677d96fc3b78.png)



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

