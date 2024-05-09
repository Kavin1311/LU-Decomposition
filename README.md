# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.Read the elements of augmented matrix into arrays a and b

2.Calculate elements of L and U

3.Print elements of L and U

4.Find V by solving LV = B by forward substitution

5.Find X by solving UX = V by backward substitution

6.Print Array X as the solution

## Program:
(i) To find the L and U matrix
'''
Program to find L and U matrix using LU decomposition.
Developed by: T.KAVINAJAI
RegisterNumber: 212223100020'''
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```

(ii) To find the LU Decomposition of a matrix
'''
Program to find L and U matrix using LU decomposition.
Developed by: T.KAVINAJAI
RegisterNumber: 212223100020'''
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),B)
print(X)
```
## Output:
![image](https://github.com/Kavin1311/LU-Decomposition/assets/145695724/a0ccc1d9-1a2f-40c5-a8c2-49b2096404e3)
![image](https://github.com/Kavin1311/LU-Decomposition/assets/145695724/5d0cfcfa-c9bb-4146-a74e-0f37351ec36b)



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

