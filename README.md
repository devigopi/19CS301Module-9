# 19CS301Module-9
### EX: 9.1                                            MATRIX OPERATIONS
### Aim: To Write a Python Program to subtract two matrices by reading the matrix from the user.
### Algorithm:

STEP 1: Start.

STEP 2: Create a variable r and c for rows and columns of the matrix.

STEP 3: Get the value of r and c from user.

STEP 4: Define a function to create a matrix.

STEP 5 : Define another function to subtract the matrices.

STEP 6: Print the result.

STEP 7 : Stop.
### Program:
```
def create_matrix(n,m):
         M = []
         for i in range(n):
                   row = []
                   for j in range(m):
                      x = int(input())
                       row.append(x)
           M.append(row)
         return M
r,c = input().split()
A = create_matrix(int(r),int(c))
B = create_matrix(int(r),int(c))
C = []
for i in range(int(r)):
         R = []
 

        for j in range(int(c)):
                item = A[i][j]-B[i][j]
   R.append(item)
C.append(R)
print(A)
print(B)
print(C)
```
### Output:
![image](https://github.com/user-attachments/assets/b1125b13-d26e-4404-acce-7dd2c1d2011c)

### Result: Thus, the given program is implemented and executed successfully .

### EX: 9.2 LIST COMPREHENSION
### Aim: To Write a Python class program to generate all even numbers between 200 and 300 and store in a list using list comprehension.
### Algorithm:
STEP 1: Start.

STEP 2: Create a class.

STEP 3: Create variable a,b, and c for upper limit,lower limit and condition.

STEP 4: Intialise the values in the class.

STEP 5 : Define a method and using list comprehension calculate the result.

STEP 6: Print the result.

STEP 7 : Stop.

### Program:
```
class program:

      def  __init__(self,a,b,c):
                self.a=a
                self.b=b
                self.c=c
        def display(self):
               even = [i for i in range(self.a,self.c+1,self.b)]
               print(even)
a = int(input())
b = int(input())
c = int(input())

obj = program(a,b,c)
obj.display()
```
### Output:
 ![image](https://github.com/user-attachments/assets/a9707d46-2d47-4472-a6b3-b407a6f6ef71)

### Result: Thus, the given program is implemented and executed successfully .

### EX: 9.3 ADVANCED LIST PROCESSING
### Aim: To Write a Python program to add two matrices using list Comprehension.

### Algorithm:

STEP 1:Initialize Matrices: Define two 2D lists (matrix1 and matrix2) of the same dimensions.
STEP2:List Comprehension:
         Outer list comprehension iterates over the rows using i.
         Inner list comprehension iterates over the columns using j.
         For each element position [i][j], sum the corresponding elements from both                    matrices:matrix1[i][j] + matrix2[i][j].
STEP 3: Store the resulting sums in a new matrix (result) of the same dimensions.

### Program:
```
def create_matrix(n,m):
    M=[]
    for i in range(n):
        row=[]
        for j in range(m):
            x=int(input())
            row.append(x)
        M.append(row)
    return M 
    
r,c=input().split()
r=int(r)
c=int(c)
A=create_matrix(r,c)
B=create_matrix(r,c)
print(A)
print(B)
T = [[A[i][j] + B[i][j] for j in range(len(A[0]))] for i in range(len(A))]
print(T)

```
### Output:

![9a](https://github.com/user-attachments/assets/a9b9ba8f-c420-4a19-8ee0-81e144c8b00a)

### Result: Thus, the given program is implemented and executed successfully .
 


### EX: 9.4       TOEPLITZ MATRIX
### Aim: To Write a Python Program to to search an element in a 2D array.


### Algorithm:
STEP 1: Start.
STEP 2:Define a 2D array (matrix) and an integer target to search for.
STEP 3:Initialize a boolean variable found to False.
STEP 4:Use a nested loop:
         Outer loop iterates through rows (i).
         Inner loop iterates through columns (j).
STEP 5:For each element matrix[i][j]:
         If it matches target, print the position (i, j) and set found = True.
         Exit the loops using break.
STEP 6:After the loop, if found is still False, print that the element is not found.
STEP 7:End


### Program:
```
def create_matrix(n,m):
    M=[]
    for i in range(n):
        row=[]
        for j in range(m):
            x=int(input())
            row.append(x)
        M.append(row)
    return M
def printmatrix(M):
    for i in range(len(M)):
        for j in range(len(M[0])):
            print(M[i][j],end=' ')
        print()
def search(M,x):
    flag=False
    for i in range(len(M)):
        for j in range(len(M[0])):
            if x==M[i][j]:
                print('Element is found in (',i,',',j,')')
                flag=True
    return flag
r,c=input().split()
A=create_matrix(int(r),int(c))
x=int(input())
printmatrix(A)
print('search element is ',x)
if (not search(A,x)):
    print('Element is not found in the Matrix')
```
### Output:


![9B](https://github.com/user-attachments/assets/0c3e2e0e-e528-4190-986e-a5d952dbad4d)

### Result: Thus, the given program is implemented and executed successfully.

9E EX: Filter the odd and even numbers

Aim:Write a Python program to filter the odd and even numbers  in a list using filter (  )

Algorithm:
Step 1:Start
Step 2:Input a list of integers (or define it in the program).
Step 3:Define a function is_even(n) that returns True if n is even.
Step 4:Define a function is_odd(n) that returns True if n is odd.
Step 5:Use filter(is_even, list) to get even numbers.
Step 6:Use filter(is_odd, list) to get odd numbers.
Step 7:Convert the filter results to lists and display them.
Step 8:End

program:
```
l=[]
n=int(input())
for i in range(n):
    x=int(input())
    l.append(x)
even_list=list(filter(lambda x: x%2==0,l))
print(even_list)
even_list=list(filter(lambda x: x%2!=0,l))
print(even_list)
```

Output:
![9e](https://github.com/user-attachments/assets/d99bbef4-05f5-4b78-a6d4-10eb160e0a84)

Result:
     Thus, the given program is implemented and executed successfully .
 

