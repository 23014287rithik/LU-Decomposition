# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm

### To find the L and U matrix:
```
Step 1: Import Numpy library as np. 
Step 2: Read a matrix A from user input.
Step 3: Perform LU decomposition of matrix A using SciPy's lu function, which returns permutation matrix P,
        lower triangular matrix L, and upper triangular matrix U.
Step 4: Print the lower triangular matrix L and the upper triangular matrix U.
```
### To find the LU Decomposition of a matrix:
```
Step 1: Read matrix A and vector b from user input. 
Step 2: Compute the LU decomposition of A using lu_factor, which returns LU matrix and pivot indices.
Step 3: Use lu_solve to solve the linear system Ax = b using the LU decomposition.
Step 4: Solution: Print the solution vector X.
```
  

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: Eesha Ranka
RegisterNumber: 212224240040
*/

import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: Eesha Ranka
RegisterNumber: 212224240040
*/

import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),b)
print(X)

```

## Output:
Output for code(i):
![image](https://github.com/user-attachments/assets/51b74520-2c7f-404b-a109-011137e1a54f)

Output for code (ii):

![image](https://github.com/user-attachments/assets/1bdff854-844c-4d44-ba5f-cf3aebaaaef6)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

