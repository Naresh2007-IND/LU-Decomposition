# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.  Import the numpy module to use the built-in functions for calculation
2. Prepare the lists from each linear equations and assign in np.array()
3. Using the np.linalg.eig(), we get two results (first is eigenvalue and second is eigenvector) of the given matrix.
4. End the program

## Program:
(i) To find the L and U matrix
```
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)

/*
Program to find the L and U matrix.
Developed by: Naresh J
RegisterNumber: 212225230195
*/
```
(ii) To find the LU Decomposition of a matrix
```
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A = np.array(eval(input()))
b = np.array(eval(input()))
lu, piv = lu_factor(A)
X = lu_solve((lu , piv),b)
print(X)

/*
Program to find the LU Decomposition of a matrix.
Developed by: Naresh J
RegisterNumber: 212225230195
*/
```

## Output:

(i)<img width="1434" height="889" alt="Screenshot 2026-03-27 141413" src="https://github.com/user-attachments/assets/2ee5ece3-5dd1-41a5-88ff-e336fa66c090" />

(ii)<img width="1254" height="830" alt="Screenshot 2026-03-27 142012" src="https://github.com/user-attachments/assets/be549edb-1ddf-4f12-970a-fdce323f86d9" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

