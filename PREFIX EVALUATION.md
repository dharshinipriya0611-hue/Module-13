# Exp.No:34  
## PREFIX EVALUATION

---

### AIM  
To write a Python program to evaluate a user-given Prefix expression using a stack. The expression must contain operators such as Multiplication, Addition, and Subtraction.

---

### ALGORITHM

1. Start the program.
2. Define a set of valid operators: *, -, +, %, /, **.
3. Initialize an empty stack.
4. Traverse the prefix expression from right to left:
5. If the character is a digit, convert it to an integer and push it onto the stack.
6. If the character is an operator, pop two elements from the stack.
7. Apply the operator on the two popped operands.
8. Push the result back onto the stack.
9. If an invalid character is encountered, raise an error.
10. After traversal, the stack should contain only one element.
11. Return the single element as the evaluation result.
12. End the program.

---

### PROGRAM
~~~
Reg.No: 212223090004
Name: D Dharshini priya

OPERATORS=set(['*','-','+','%','/','**']) 
def evaluate(expression):
	stack = []
	for c in expression[::-1]:
		if c not in OPERATORS:
			stack.append(int(c))
		else:
			o1 = stack.pop()
			o2 = stack.pop()
			if c == '+':
				stack.append(o1 + o2)
			elif c == '-':
				stack.append(o1 - o2)
			elif c == '*':
				stack.append(o1 * o2)
	return stack.pop()    
test_expression = input()
print("Prefix Expression :",test_expression)
print("Evaluation result :", evaluate(test_expression))
~~~


### OUTPUT
<img width="819" height="244" alt="image" src="https://github.com/user-attachments/assets/b6bbcdae-00cc-413e-9c0a-1a07d1ba80ca" />




### RESULT
Thus the program is created and verified successfully.
