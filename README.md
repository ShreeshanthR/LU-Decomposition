# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Read the input matrix (and RHS vector if required).
2. Perform LU decomposition of the matrix using SciPy LU decomposition method.
3. Separate and obtain the Lower triangular matrix L and Upper triangular matrix U.
4. Display the L, U matrices (and solve the system using LU decomposition if required).

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: Shreeshanth R
RegisterNumber: 212225040411
*/

import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U = lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: Shreeshanth R
RegisterNumber: 212225040411
*/

import numpy as np
from scipy.linalg import lu_factor, lu_solve
A = np.array(eval(input()))
B = np.array(eval(input()))
lu, pivot = lu_factor(A)
x = lu_solve((lu,pivot),B)
print(x)
```

## Output:
(i)
<img width="1227" height="473" alt="image" src="https://github.com/user-attachments/assets/6400ec4e-e17e-4c8b-a7fb-48888a3d6634" />
(ii)
<img width="917" height="210" alt="image" src="https://github.com/user-attachments/assets/d7fb2a60-1de7-4614-8d03-dd87c189f1ff" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

