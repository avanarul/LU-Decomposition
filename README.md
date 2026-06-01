# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
Step 1: Import the required libraries such as NumPy and SciPy.
Step 2: Define the matrix using np.array() and store it in a variable.
Step 3: Use the scipy.linalg.lu() function to perform LU Decomposition and obtain the lower triangular matrix (L), upper triangular matrix (U), and permutation matrix (P).
Step 4: Display the matrices P, L, and U using the print() function.
## Program:
(i) To find the L and U matrix
```

/*
Program to find the L and U matrix.
Developed by: s avan arul
RegisterNumber: 212225040036
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
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
Developed by: s avan arul
RegisterNumber:212225040036
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()),dtype='i')
B=np.array(eval(input()),dtype='i')
X=lu_factor(A)
solution=lu_solve(X,B)
print(solution)

```

## Output:
<img width="1229" height="571" alt="image" src="https://github.com/user-attachments/assets/fa3a3a2c-4e6b-412f-b5f8-d8733282150e" />
<img width="1009" height="325" alt="image" src="https://github.com/user-attachments/assets/6d70b480-b3f9-4cd1-b896-7926b5fa7549" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

