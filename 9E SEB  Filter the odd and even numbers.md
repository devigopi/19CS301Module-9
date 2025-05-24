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

