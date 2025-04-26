# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### Step 1:  
Import the necessary libraries: numpy and lu function from scipy.linalg.

### Step 2:  
Define the matrix A using np.array() with given elements. 

### Step 3:  
Perform LU decomposition using lu(A) to get matrices P, L, and U. 

### Step 4:  
Display the matrices L, and U using print().  

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

