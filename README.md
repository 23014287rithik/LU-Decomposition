# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import required libraries numpy and scipy.linalg.

2. Input the matrix/matrices using eval(input()).

3. Perform LU decomposition using lu() or solve equations using lu_factor() and lu_solve().

4. Print the results L and U matrices or solution X matrix.

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: RITHIK V
RegisterNumber: 212223230171
import numpy as np
from scipy.linalg import lu
a=np.array(eval(input()))
p,l,u=lu(a)
print(l)
print(u)
*/
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: RITHIK V
RegisterNumber: 212223230171
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(a)
x=lu_solve((lu,piv),b)
print(x)
*/
```

## Output:
![image](https://github.com/user-attachments/assets/0f361ef9-656c-4544-bb66-1ada09a679a7)

![image](https://github.com/user-attachments/assets/4ef70ad4-db88-4984-a8ad-cfda2f540df0)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.
