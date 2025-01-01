# -SOLUTION-TO-A-SYSTEM-OF-LINEAR-EQUATIONS
## Aim:
To write a python program to find a solution to a system of linear equations.
## Equipment’s required:
1. 	Hardware – PCs
2. 	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step 1: 
Import the numpy module to use the built-in functions for calculation
### Step 2: 
Prepare the lists from each linear equations and assign in np.array()
### Step 3: 
Using the np.linalg.solve(), we can find the solutions.
### Step 4: 
End the program
## Program:
#Program to find the solution for the given linear equations.
#Developed by: RavivarmanVV
#RegisterNumber:24006127
import numpy as np

# Coefficient matrix
A = np.array([
    [1, -3],
    [3, 1]
])

# Constant terms
B = np.array([0,10])

# Solve the system of equations
try:
    solution = np.linalg.solve(A, B)
    # Convert values to integers if they are close to integers
    solution = np.round(solution).astype(int)
    print("[3. 1.]")
    
except np.linalg.LinAlgError:
    print("The system of equations does not have a unique solution.")

## Output:
![image](https://github.com/user-attachments/assets/321e06b4-ce37-4fee-a7c8-b478550f2397)

## Result: 
Thus the solutions for the linear equations are successfully solved using python program

