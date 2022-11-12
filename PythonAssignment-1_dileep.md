## Assignment Part-1
Q1. Why do we call Python as a general purpose and high-level programming language?

-->> Python is a multi domain programming language like for developing websites and software, task automation, data analysis,data visualization, data engineering , data science etc.
    A general-purpose language is a programming language that is capable of creating all types of programs. 
	A language that is not a general-purposed language is called a DSL (domain-specific language)

-->> A high-level language is any programming language that enables development of a program in a much more user-friendly programming context 
    and is generally independent of the computer's hardware architecture.
    A high-level language has a higher level of abstraction from the computer, and focuses more on the programming logic rather than 
   the underlying hardware components such as memory addressing and register utilization.

Q2. Why is Python called a dynamically typed language?

-->> Because python doesn’t know about the type of the variable until the code is run. So declaration is of no use.As it will get to know the type of the value at run-time.


Q3. List some pros and cons of Python programming language?

Pros --> Python is easy to learn and read 
	Python enhances productivity
	Python has a vast collection of libraries
	Python is free, open-source, and has a vibrant community
	Python is a portable programming language
	Python is an interpreted language
	
Cons --> Python has speed limitations
		Python is not so strong with mobile computing
		Python can have runtime errors
		Python consumes a lot of memory space
		Python is not easy to test
		
Q4. In what all domains can we use Python?

--> Machine learning / Artificial intelligence
	Desktop GUI
	Data (Analytics/visualization/Engineering/science ) etc 
	Web development
	Game development
	Mobile app development
	Embedded systems

Q5. What are variable and how can we declare them?

--> Python has no command for declaring a variable. A variable is created the moment you first assign a value to it.
	Python variables are of four different types: Integer, Long Integer, Float, and String.

Q6. How can we take an input from the user in Python?

---> val = input("Enter your value: ")
	 print(val)

Q7. What is the default datatype of the value that has been taken as an input using input() function?

--> Python input() function is used to take user input. By default, it returns the user input in form of a string.


Q8. What is type casting?

--> Type Casting is the method to convert the variable data type into a certain data type in order to the operation required to be performed by users.

Q9. Can we take more than one input from the user using single input() function? If yes, how? If no, why?

--> YES.
in Python user can take multiple values or inputs in one line by two methods. 
Using split() method
input().split(separator, maxsplit)

# taking multiple inputs at a time 
# and type casting using list() function
x = list(map(int, input("Enter multiple values: ").split()))
print("List of students: ", x)

Using List comprehension

Q10. What are keywords?

--> Python keywords are special reserved words that have specific meanings and purposes and can't be used for anything but those specific purposes.

Q11. Can we use keywords as a variable? Support your answer with reason.

--> We cannot use a keyword as a variable name, function name, or any other identifier. They are used to define the syntax and structure of the Python language. 
    All the keywords except True , False and None are in lowercase and they must be written as they are.
	
Q12. What is indentation? What's the use of indentaion in Python?

-->  Indentation refers to the spaces at the beginning of a code line. Where in other programming languages the indentation in code is for readability only, the indentation in Python is very important. 
     Python uses indentation to indicate a block of code.

Q13. How can we throw some output in Python?

-->  The basic way to do output is the print statement. To end the printed line with a newline, add a print statement without any objects. 
     This will print to any object that implements write(), which includes file objects.

Q14. What are operators in Python?

--> Operators are special symbols in Python that carry out arithmetic or logical computation. The value that the operator operates on is called the operand. 
	In Python, there are seven different types of operators: arithmetic operators, assignment operators, comparison operators, logical operators, identity operators, membership operators, 
	and boolean operators.
	
Q15. What is difference between / and // operators?

--> In Python programming, you can perform division in two ways. The first one is Float Division("/") and the second is Integer Division("//") or Floor Division.

Q16. Write a code that gives following as an output.

```
iNeuroniNeuroniNeuroniNeuron
```

--> 
print ("'''")
print('iNeuron'*4)
print ("'''")

Q17. Write a code to take a number as an input from the user and check if the number is odd or even.

--> num = int(input("Enter a number: "))
if (num % 2) == 0:
   print("{0} is Even".format(num))
else:
   print("{0} is Odd".format(num))

Q18. What are boolean operator?

--> Boolean Operators are those that result in the Boolean values of True and False. These include and, or and not. While and & or require 2 operands, not is a unary operator.
    Boolean operators are most commonly used in arithmetic computations and logical comparisons.

Q19. What will the output of the following?
```
1 or 0    --> 1

0 and 0   --> 0 

True and False and True --> False

1 or 0 or 0  --> 1
```

Q20. What are conditional statements in Python?

--> A conditional statement as the name suggests itself, is used to handle conditions in your program. 
	These statements guide the program while making decisions based on the conditions encountered by the program. 
	Python has 3 key Conditional Statements that you should know: if statement. if-else statement.
	
	--> Conditional Statement in Python perform different computations or actions depending on whether a specific Boolean constraint evaluates to true or false. 
	    Conditional statements are handled by IF statements in Python.

Q21. What is use of 'if', 'elif' and 'else' keywords?

--> Python if Statement is used for decision-making operations. It contains a body of code which runs only when the condition given in the if statement is true. 
    If the condition is false, then the optional else statement runs which contains some code for the else condition.
    When you want to justify one condition while the other condition is not true, then you use Python if else statement.


Q22. Write a code to take the age of person as an input and if age >= 18 display "I can vote". If age is < 18 display "I can't vote".

age = int(input("Enter your age: "))
if (age >= 18):
   print("i can vote" )
else:
   print("i can't vote")


Q23. Write a code that displays the sum of all the even numbers from the given list.
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```
# list of numbers
list1 = [12, 75, 150, 180, 145, 525, 50]

# using list comprehension
even_nos = [num for num in list1 if num % 2 == 0]

print("sum of even numbers in the list: ",sum(even_nos))

Q24. Write a code to take 3 numbers as an input from the user and display the greatest no as output.

num1 = int(input("Enter number 1: "))
num2 = int(input("Enter number 2: "))
num3 = int(input("Enter number 3: "))
allNum = [num1, num2, num3]
maxNum = max(allNum)
maxIndex = allNum.index(max(allNum))
print("Greatest number is number "+str(maxIndex+1))


Q25. Write a program to display only those numbers from a list that satisfy the following conditions

- The number must be divisible by five

- If the number is greater than 150, then skip it and move to the next number

- If the number is greater than 500, then stop the loop
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```					

# list of numbers
list1 = [12, 75, 150, 180, 145, 525, 50]

for num in list1:
    if num > 500:
        break;
    if num % 5 == 0 and num <= 150:
        print(num,"");
