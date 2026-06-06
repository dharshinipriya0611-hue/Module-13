# Exp.No:31  
## IMPLEMENTATION OF STACK

---

### AIM  
To write a Python program to implement a stack using a list and its built-in methods (`append()`, `pop()`).

---

### ALGORITHM
---
1. Start the program.
2. Initialize an empty list called stack.
3. Repeat 5 times (for i = 1 to 5):
4. Take input from the user.
5. Append the input to the stack using append().
6. Display "Stack before elements are popped".
7. Print the current contents of stack.
8. Repeat 2 times (for i = 1 to 2):
9. Remove the last element from the stack using pop().
10. Display "Stack after elements are popped".
11. Print the updated contents of stack.
12. End the program.**
---

### PROGRAM

~~~
Reg.no: 212223090004
Name: D Dharshini priya

stack = []
for i in range (5):
    a=input()
    stack.append(a)
print("Stack before elements are popped")
print(stack)
print()
for i in range(2):
    stack.pop()
print('Stack after elements are popped:')
print(stack)
~~~

### OUTPUT
<img width="1519" height="700" alt="image" src="https://github.com/user-attachments/assets/5cd65675-49a0-4a8e-bc76-c5e16b69ee8c" />

### RESULT
Thus the program is created and verified.

