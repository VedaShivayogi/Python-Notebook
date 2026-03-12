<b><h1>Python Essentials for Automation and AI Agents</h1></b>
<p> Python is a high-level, interpreted, object-oriented programming language (created by Guido van Rossum, 1991).</p>

* Python is **easy to read and write**
* Works on **Windows, Linux, and macOS**
* Has **many built-in libraries**
* Used in **Automation, AI, Data Science, Web Development, and Networking**
* Supports **procedural**, **object-oriented**, and **functional** programming
  
<details>
<b><summary>Introduction</summary></b>
<h3>Indentation in python</h3>

* In Python, **indentation is used to define blocks of code**.
* It tells the Python interpreter that a **group of statements belongs to the same block**.
* Unlike other languages, Python **does not use braces `{}`** to define blocks.
* **All statements with the same level of indentation** are treated as part of the **same block**.
* The most common convention is to use **4 spaces (or one tab)** for each level of indentation.
</details>



<h2>Data types and variables</h2>
<details>
<summary>Show more</summary>

### <b> Variables in Python </b>

* Variables are used to **store data** in a program.
* They are **dynamically typed**, meaning you do **not** need to specify the data type.
* A variable can be **referenced and modified** while the program is running.
* A variable is simply a **name given to a value**.
* In Python, the **type is automatically decided** based on the value assigned.

###  Rules for Naming Variables 

* Variable names can contain **letters (a–z, A–Z)**, **digits (0–9)**, and **underscores (_)**.
* A variable name **cannot start with a digit**.
* Variable names are **case-sensitive**, so `myVar` and `myvar` are **different**.
* **Python keywords** such as `if`, `else`, `for`, `while`, etc., **should not be used** as variable names.

###  Valid Variable Names
``` python
age = 20
student_name = "Reva"
marks1 = 85
_total = 100
```
###  Invalid Variable Names
``` python
1name = "Reva"      # Cannot start with digit <br>
my-name = 10       # Hyphen not allowed <br>
for = 5            # 'for' is a Python keyword <br>
```


#### Basic Data types:
| Type | Example|
|------|--------|
|int   | 10     |
|float   | 3.14     |
|str   | "hello" or 'hello'     |
|bool   | `True` / `False`    |
|list   | [1,2,3]     |
|tuple   | (1,2,3)     |
|dict   | {"name":"Alex"}     |



# Example 
# Assigning values to variables
a = 10          # Integer
b = 3.14        # Float
c = "Python"    # String
d = True        # Boolean
e=[1,2,3]
f=(1,2,3)
g={"clg_name":"Reva"}
# Printing values
print(a)
print(b)
print(c)
print(d)
print(e)
print(f)
print(g)

#  Checking Variable Types
print(type(a))
print(type(b))
print(type(c))
print(type(d))
print(type(e))
print(type(f))
print(type(g))
#Dynamic Typing Example
v = 5
print(v, type(v))

v = "Hello"
print(v, type(v))
<h2>Python Keywords</h2>
<details>
<summary>Show more</summary>

###  Keywords in Python 

* **Keywords are reserved words** in Python.
* They have a **special meaning** and are used to define the **rules and structure** of Python programs.
* In Python, **keywords are case-sensitive**.
* **Keywords cannot be used** as names for:
  * variables
  * functions
  * classes
  * or any other identifiers


import keyword
print("The list of keywords are : ")
print(keyword.kwlist)
print(len(keyword.kwlist))
<details>
<summary>Show more</summary>
    
###  Python Keywords 

* In **Python 3.3**, there were **33 keywords**.
* Over time, this number can change.
* Currently, there are **35 keywords** in Python (as shown by output).
* All keywords are written in **lowercase**, **except**:

  * `True`
  * `False`
  * `None`
* Keywords **cannot be used** as:

  * variable names
  * function names
  * class names
  * or any other identifiers
* Keywords are used to **define the syntax and structure** of the Python language.

###  Identifying Python Keywords 

**1. Syntax Highlighting**

* In editors or Jupyter Notebook, keywords appear in a **different color or style**.

**2. SyntaxError**

* If a keyword is used incorrectly, Python will show a **SyntaxError**.


| Category                  | Keywords                                                                 |
|---------------------------|--------------------------------------------------------------------------|
| Value Keywords            | True, False, None                                                        |
| Operator Keywords         | and, or, not, is, in                                                      |
| Control Flow Keywords     | if, else, elif, for, while, break, continue, pass, try, except, finally, raise, assert |
| Function and Class        | def, return, lambda, yield, class                                        |
| Context Management        | with, as                                                                 |
| Import and Module         | import, from                                                             |
| Scope and Namespace       | global, nonlocal                                                         |
| Async Programming         | async, await                                                             |

<h2>Input and Output in Python</h2>
<details>
<summary>Show more</summary>

- **print()** function can display output in various formats.
- **input()** function enables interaction with users by gathering input during program execution.
<h2>Python Operators</h2>
<details>
<summary>Show more</summary>

_In Python programming, Operators in general are used to perform operations on values and variables._

- Operators: Special symbols like -, + , * , /, etc.
- Operands: Value on which the operator is applied.

  1. Arithmetic Operators
  2. Relational Operators
  3. Assignment Operators 
  4. Logical Operators
  5. Membership Operators
  6. Identity Operators 
  7. Bitwise Operators


| Type                   | Operators                     |
|------------------------|-------------------------------|
| Arithmetic Operators   | +, -, *, /, %                 |
| Relational Operators   | <, <=, >, >=, ==, !=, <>      |
| Logical Operators      | AND, OR, NOT                  |
| Bitwise Operator       | &, |, ^, ~, <<, >>            |
| Assignment Operator    | =, +=, -=, *=, %=             |

<h5>1. Arithmetic Operators</h5>
<details>
<summary>Show more</summary>
a=5 <br> b=10
    
_Python Arithmetic operators are used to perform basic mathematical operations like addition, subtraction, multiplication and division._

| Operator | Example Expression | Result |
|----------|--------------------|--------|
| +        | a + b              | 15     |
| -        | a - b              | 5      |
| *        | a * b              | 50     |
| /        | a / b              | 2      |
| %        | a % b              | 0      |

a = 9
b = 8

# Addition
print("Addition:", a + b)  

# Subtraction
print("Subtraction:", a - b) 

# Multiplication
print("Multiplication:", a * b)  

# Division
print("Division:", a / b) 

# Floor Division
print("Floor Division:", a // b)  

# Modulus
print("Modulus:", a % b) 

# Exponentiation
print("Exponentiation:", a ** b)
<h5>2. Comparison Operators</h5>
<details>
<summary>Show more</summary>

_In Python, Comparison (or Relational) operators compares values. It either returns True or False according to the condition._

| Operator | Description                         |
|----------|-------------------------------------|
| <        | Less than                            |
| >        | Greater than                         |
| <=       | Less than or equal to                |
| >=       | Greater than or equal to             |
| ==       | Equal to                             |
| !=       | Not equal to                         |
| <>       | Not equal to (similar to !=)         |


a = 11
b = 7
c=7
print(a > b)
print(a < b)
print(a == b)
print(c == b)
print(a != b)
print(a >= b)
print(a <= b)
<h5>3. Logical Operators</h5>
<details>
<summary>Show more</summary>

_Python Logical operators perform Logical AND, Logical OR and Logical NOT operations. It is used to combine conditional statements._

The precedence of Logical Operators in Python is as follows:

1. Logical not
2. Logical and
3. Logical or

a = True
b = False
print(a and b)
print(a or b)
print(not a)
<h5>4. Bitwise Operators</h5>
<details>
<summary>Show more</summary>

_Python Bitwise operators act on bits and perform bit-by-bit operations. These are used to operate on binary numbers._

Bitwise Operators in Python are as follows:

1. Bitwise NOT
2. Bitwise Shift
3. Bitwise AND
4. Bitwise XOR 
5. Bitwise OR
a = 10
b = 4

print(a & b)
print(a | b)
print(~a)
print(a ^ b)
print(a >> 2)
print(a << 2)
<h5>5. Assignment Operators</h5>
<details>
<summary>Show more</summary>

_Python Assignment operators are used to assign values to the variables. This operator is used to assign the value of the right side of the expression to the left side operand._


| Operator | Description                   |
|----------|-------------------------------|
| =        | Assignment                    |
| /=       | Divide and assign             |
| +=       | Add and assign                |
| -=       | Subtract and assign           |
| *=       | Multiply and assign           |
| %=       | Modulus and assign            |
| **=      | Exponent and assign           |
| //=      | Floor division and assign     |

a = 8
b = a
print(b)
b += a
print(b)
b -= a
print(b)
b *= a
print(b)
b <<= a
print(b)
<h5>6. Identical Operators</h5>
<details>
<summary>Show more</summary>

_In Python, is and is not are the identity operators both are used to check if two values are located on the same part of the memory. Two variables that are equal do not imply that they are identical._ 

``` python 
is          # True if the operands are identical 
is not      # True if the operands are not identical
```
a = 10
b = 20
c = a

print(a is not b)
print(a is c)
<h5>7. Membership Operators</h5>
<details>
<summary>Show more</summary>

_In Python, in and not in are the membership operators that are used to test whether a value or variable is in a sequence._<br>
``` python
in            # True if value is found in the sequence<br>
not in        # True if value is not found in the sequence
```
x = 24
y = 20
list = [10, 20, 30, 40, 50]

if (x not in list):
    print("x is NOT present in given list")
else:
    print("x is present in given list")

if (y in list):
    print("y is present in given list")
else:
    print("y is NOT present in given list")
<h5>8. Ternary Operators</h5>
<details>
<summary>Show more</summary>

_in Python, Ternary operators also known as conditional expressions are operators that evaluate something based on a condition being true or false. It was added to Python in version 2.5._ 

*It simply allows testing a condition in a single line replacing the multiline if-else, making the code compact.*

> Syntax :  [on_true] if [expression] else [on_false] 
a, b = 11, 8
min = a if a < b else b

print(min)
<h2>Comment Lines</h2>
<details>
<summary>Show more</summary>
    
* **Comments are used to explain the code**.
* They make the program **easy to read and understand**.
* **Python ignores comments** while executing the program.


### 1️ Single-Line Comments
* Single-line comments start with the **`#` symbol**.
* They are used to explain a single line of code.

```python
# This is a single-line comment
x = 10  # This comment explains the variable
```
# This is a single-line comment
``` python
x = 10  # This comment explains the variable
```
### 2️ Multi-Line Comments

* Python does **not** have a special multi-line comment symbol.
* Multi-line comments are written using **multiple `#` symbols**.
``` python
#This is a multi-line comment
#written using multiple
#single-line comments
```

### 3️ Docstrings (Documentation Strings)

* **Docstrings are used to document**:

  * functions
  * classes
  * modules
* They are written using **triple quotes** (`'''` or `"""`).
``` python
def add(a, b):
    """
    This function adds two numbers
    and returns the result.
    """
    return a + b
```
###  Note

* Docstrings can be accessed using `help()` or `__doc__`.


print(add.__doc__)

<h2>Conditional Statements in Python</h2>

- Conditional statements in Python are used to execute certain blocks of code based on specific conditions. 
- These statements help control the flow of a program, making it behave differently in different situations.

<h5>If Conditional Statement</h5>
<details>
<summary>Show more</summary>
If statement is the simplest form of a conditional statement. It executes a block of code if the given condition is true.

**Syntax**
``` python
if condition:
    # body of if statement
```
Here, `condition` is a boolean expression, such as number > 5, that evaluates to either ```True``` or ```False```.

- If `condition` evaluates to `True`, the body of the if statement is executed.
- If `condition` evaluates to `False`, the body of the if statement will be skipped from execution.

#### Working of if statement:
# Example 
number = int(input('Enter a number: '))

# check if number is greater than 0
if number > 0:
    print(f'{number} is a positive number.')

print('A statement outside the if statement.')
<h5>Python if...else statement</h5>
<details>
<summary>Show more</summary>

An `if` statement can have an optional `else` clause. The `else` statement executes `if` the condition in the if statement evaluates to `False`.

**Syntax**
``` python
if condition:
    # body of if statement
else:

    # body of else statement
```
Here, if the condition inside the if statement evaluates to

- **True** - the body of if executes, and the body of else is skipped.
- **False** - the body of else executes, and the body of if is skipped
# Example 
num=int(input("Enter the number"))

if num > 0:
    print('Positive number')

elif num < 0:
    print('Negative number')

else:
    print('Zero')

print('This statement is always executed')
<h5>Python Nested if statement</h5>
<details>
<summary>Show more</summary>

**Nested if..else** means an if-else statement inside another if statement. We can use nested if statements to check conditions within conditions.

# Example 
number = int(input("Enetr the number"))

# outer if statement
if number >= 0:
    # inner if statement
    if number == 0:
      print('Number is 0')
    
    # inner else statement
    else:
        print('Number is positive')

# outer else statement
else:
    print('Number is negative')
<h3>Class Exercise - 1</h3>
<h4>Sort the files to directories based on extensions</h4>
<details>
<summary>Show more</summary>

**Steps:**
- Input `file_name`
- Finds the last occuring `.<extension_name>`
- Store the `.<extension_name>` in a variable.
- Move files to the categorized directory using if-else statements.

# Solution 
file_input = input("Enter file name: ")
extension=file_input.rfind(".")
file_type=file_input[extension:]

if(file_type == ".pdf"):
  print(f"moving file type {file_type} to Docs")
    
elif(file_type == ".jpg"):
  print(f"Moving file type {file_type} to Images")
    
elif(file_type == ".png"):
  print(f"Moving file type {file_type} to Images")
    
else:
  print(f"Invalid file type {file_type} Moving to others")
<h3>Class Exercise - 2</h3>
<h4>Washing Machine problem</h4>
<details>
<summary>Show more</summary>

A washing machine works on the principle of `Fuzzy System`, the weight of the clothes put inside it for washing is uncertain. But based on weight measured by sensors, it decides time and water level which can be changed by menus given on the machine control area.

> For **low level** water, the time estimate is `25 minutes`, where approximately weight is between `2000` grams or any nonzero positive number below that.

> For **medium level** water, the time estimate is `35 minutes`, where approximately weight is between `2001` grams and `4000` grams.

> For **high level** water, the time estimate is `45 minutes`, where approximately weight is between `4000` grams and `7000` grams.

Assume the capacity of the machine is maximum `7000` grams.
Where approximately weight is zero, time estimate is 0 minutes.
# Solution 1
cloth_weight = float(input("Enter the Weight of the clothes: "))
if (cloth_weight > 0):
  if(cloth_weight<2000):
    print(f"For the {cloth_weight}, Requires low level of water, Estimated time of wash is 25 mins")
  elif(cloth_weight >= 2000 and cloth_weight<4000):
    print(f"For the {cloth_weight}, Requires Medium Water level. Estimated time of wash is 35 mins")
  elif(cloth_weight>= 4000 and cloth_weight<7000):
    print(f"For the {cloth_weight}, Requires High level of water. Estimated time of wash is 45 mins")
  else:
    print(f"{cloth_weight} Weight Overload!")
else:
  print(f"The Weight is {cloth_weight} Est. time is 0 minutes")
# Solution 2 using in-range
cloth_weight = float(input("Enter the Weight of the clothes: "))
if cloth_weight > 0:
  if cloth_weight in range(1,2000):
    print(f"For the {cloth_weight}, Requires low level of water, Estimated time of wash is 25 mins")
  elif cloth_weight in range(2000,4000):
    print(f"For the {cloth_weight}, Requires med level of water, Estimated time of wash is 35 mins")
  elif cloth_weight in range(4000,7000):
    print(f"For the {cloth_weight}, Requires high level of water, Estimated time of wash is 45 mins")
  else:
    print(f"{cloth_weight} weight overloaded!")
else:
  print(f"For the {cloth_weight}, Estimated time of wash is 0 mins")
<h3>Class Exercise - 3</h3>
<h4>Employee Performance Rating System</h4>
<details>
<summary>Show more</summary>

*Using condtional statements*

### Problem Scenario (HR Automation Case Study):

A multinational company is automating its annual employee appraisal process. Each employee receives a perfoemance score between 0 an 100, based on multiple evaluation parameters like teamwork, communication, KPI achievements and innovation. The HR wants an automated system (Python-based) that takes `employee name` and `score` as input and outputs.


| Score Range  | Rating         | Appraisal Eligibility          |
|--------------|----------------|--------------------------------|
| 90-100 | Outstanding | Eligible for high appraisal|
| 75-89 | Excellent | Eligible for moderate appraisal|
| 60-74 | Good | Eligible for basic appraisal|
| 40-59 | Needs Improvement | Not Eligible |
| Below 40 | Poor | Not Eligible & training Required |


name_var = input("Enter the employee name : ")
score_var = int(input("Enter the score of the employee: "))
print(f"-------------------------------\nEmployee {name_var} has a score : {score_var}")

if(score_var > 0 and score_var<101):
  if score_var in range(40,59):
    print(f"Rating : Needs Improvement,\nAppraisal Status:  Not eligible")

  elif score_var in range(60,74):
    print(f"Rating : Good, \nAppraisal Status:  Eligible for Basic Appraisal")

  elif score_var in range(75,89):
    print(f"Rating : Excellent, \nAppraisal Status:  Eligible for Moderate Appraisal")

  elif score_var in range(90,101):
    print(f"Rating : Outstanding, \nAppraisal Status:  Eligible for High Appraisal\nConsidered for leadership and International opportunities")

  else:
    print(f"Rating : Poor, \nAppraisal Status:  Not eligible & training required")

else:
  print("Invalid input")
<h3>Class Exercise - 4</h3>
<h4>Scenario Based Problem - Fuel Efficiency indicator</h4>
<details>
<summary>Show more</summary>

A leading automobile conpany is developing a Python-based tool to analyze vehicle fuel efficiency. A remote IoT sensor collects the `distance travelled (km)` and `fuel consumed (litres)` after each trip. Based on the `fuel economy (km/l)`, the system must classify the vehicle's efficiency and provide suggestions.

Inputs:
- Take `distance (km)` and `fuel used (litres)` as input.
- Calculate `fuel efficiency` using:
  - Fuel Efficiency = Distance /Fuel used.

| Efficiency | Category | Suggested Action |
|------------|----------|------------------|
| >=20 | Excellent | Optimal engine performance |
| 15-19 | Good | No action needed |
|10 -14 | Needs Maintenance| Tune Engine required|
|<10 | Critical | Immediate inspection |
vechicle_id = input("Enter Vehicle ID (Ex: TN12AB0010) : ")  
distance_travelled = float(input("Enter Distance (km) : "))
fuel_used = float(input("Fuel used (litres) :"))

fuel_efficiency = distance_travelled/fuel_used

print(f"----------------------------------------\nFuel Efficiency Report\n----------------------------------------\nVehicle: {vechicle_id}\nDistance Travelled : {distance_travelled} km\nFuel used : {fuel_used} liters\nEfficiency : {round(fuel_efficiency,2)} km/l")

if (fuel_efficiency >=20):
  print(f"Efficiency Category : 🚀Excellent\nSuggested Action: Engine performance optimal. No action required ")

elif(fuel_efficiency in range(15,20)):
  print(f"Efficiency Category : Good\nSuggested Action: No action needed ")

elif(fuel_efficiency in range(10,15)):
  print(f"Efficiency Category : Needs Maintenance\nSuggested Action:Tune Engine required")

elif(fuel_efficiency in range(0,10)):
  print(f"Efficiency Category : Critical\nSuggested Action: Immediate inspection ")

else:
  print("Efficiency Category : Invalid \nSuggested Action: <Re-enter details> ")
print("----------------------------------------")
<h2>Looping Statements</h2>
<details>
<summary>Show more</summary>
    
 1. For
 2. While
 3. Nested loop


<h5>  For Loop </h5>
<details>
<summary>Show more</summary>


* A **for loop** is used to **repeat a block of code**.
* It is mainly used to **iterate over a sequence** like:

  * list
  * tuple
  * string
  * range of numbers
* It works like an **iterator**, taking **one value at a time** from the sequence.

###### <b> Syntax</b>
```python
for variable in sequence:
    statement(s)
```

###### <b> Explanation </b>
* `for` → loop keyword
* `variable` → takes one value at a time
* `sequence` → list, tuple, string, or range
* `statement(s)` → code to be repeated


# Example
for i in range(5):
    print(i)
# Example
fruits = ["apple", "banana", "mango"]

for fruit in fruits:
    print(fruit)
<h5>  While Loop </h5>
<details>
<summary>Show more</summary>

• A **while loop** is used to execute a block of statements **repeatedly**  
• The loop continues **as long as the condition is true**  
• When the condition becomes **false**, the loop stops  

###### <b> Syntax</b>

```python
while <condition>:
    statement(s)
```

* `while` → keyword
* `<condition>` → condition till which loop repeats
* ` Statement(s)` must be indented
</details>
  
<details>
<summary>Explanation Example 1 : while Loop</summary>

* a = 5 → initialization
* a <= 25 → condition check
* Loop runs while condition is true
* print(a, end=" ") prints values in same line
* a = a + 5 updates the value
* Loop stops when condition becomes false
#Example 1 : while Loop
a = 5

while a <= 25:
    print(a, end=" ")
    a = a + 5

<h5> Nested Loops </h5>
<details>
<summary>Show more</summary>

* A **Nested Loop** is a loop **inside another loop**.  
* The **outer loop** controls rows, the **inner loop** controls columns or repeated statements.  
* The inner loop runs completely for **each iteration** of the outer loop.

###### <b> Syntax </b>

**Nested for loop:**
```python
for outer_var in sequence:
    for inner_var in sequence:
        statement(s)
```

**Nested while loop:**
while condition1:
    while condition2:
        statement(s)
</details>
<details>
<summary>Explanation Example 1 : <b>  Program to print a pattern </b> </summary>
    
* Outer loop i runs 1 to 5 → controls rows
* Inner loop j runs 1 to i → prints number i multiple times in each row
* print(i, end=" ") → prints numbers in the same line
* print() → moves to the next line after each row

| Value of `i` | Inner loop runs | Output    |
| ------------ | --------------- | --------- |
| 1            | 1 time          | 1         |
| 2            | 2 times         | 2 2       |
| 3            | 3 times         | 3 3 3     |
| 4            | 4 times         | 4 4 4 4   |
| 5            | 5 times         | 5 5 5 5 5 |



# Program to print a pattern
for i in range(1, 6):
    for j in range(1, i + 1):
        print(i, end=" ")
    print()

<h2> Break , Continue and Pass Statements </h2>
<details>
<summary>Show more</summary>
    
##### <b> Break Statement</b>
* The **break statement** is used to **stop a loop** before it finishes all iterations.  
* When `break` is encountered:
  - The loop **stops immediately**  
  - The program continues with the **first line after the loop**

###### <b> Syntax </b>

```python
for variable in sequence:
    if condition:
        break
    statement(s)
```
</details>
<details>
<summary>Explanation Example 1 : </summary>
    
###### <b> Example of the breaks </b>
<b> Example 1
* for i in range(1,6) → i takes values 1,2,3,4,5
* if i == 4: → condition to stop the loop
* print("loop breaks") → prints message when loop stops
* break → exits the loop immediately
* print(i, end=" ") → prints numbers before 4

<br>
</details>
<details>
<summary>Explanation Example 2 : </summary>
    
<b> Example 2 Break in Inner Loop </b>

* Outer loop i runs from 1 to 5 → controls rows
* Inner loop j runs from 1 to 3 → controls columns
* if j == 3: → stops inner loop when j is 3
* print(i, end=" ") → prints the outer loop value before breaking
* print() → moves to next line after inner loop
* The outer loop continues, inner loop breaks at j==3.
</details>
<details>
<summary>Explanation Example 3 :  </summary>
    
<b> Example 3 Break in Outer Loop </b>

* Outer loop i runs 1 to 5
* if i == 3: → break stops the outer loop completely
* Inner loop prints 3 numbers for each i
* Loop stops entirely at i == 3
</details>

# example 1
for i in range(1, 6):
    if i == 4:
        print("loop breaks")
        break
    print(i, end=" ")
# Example 2 Break in Inner Loop
for i in range(1, 6):
    for j in range(1, 4):
        if j == 3:
            print("loop breaks")
            break
        print(i, end=" ")
    print()

# Example 3 Break in Outer Loop
for i in range(1, 6):
    if i == 3:
        print("loop breaks")
        break
    for j in range(1, 4):
        print(i, end=" ")
    print()

<h5>  Continue Statements </h5>
<details>
<summary>Show more</summary>
    
* The **continue statement** is used to **skip the current iteration** of a loop.  
* When `continue` is encountered:
  - The rest of the code in the **current iteration is skipped**  
  - The loop **moves to the next iteration**  
* Works with **for loops** and **while loops**  
* In **nested loops**, `continue` affects **only the loop in which it appears**
</details>
<h6><b>Example 1 : Simple Loop</b></h6>
<details>
<summary>Explanation Example 1 </summary>

* i goes from 1 to 5
* When i == 4, continue is executed
* The print(i) is skipped for i == 4
* Loop continues with next iteration (i = 5)
</details>
<h6><b>Example 2 : Nested Loop</h6>
<details>
<summary>Explanation Example 2 </summary>

* Outer loop i runs 1 to 5 → controls rows
* Inner loop j runs 1 to 3 → controls columns
* if j == 2: continue → skips printing 2
* print(j, end=" ") → prints remaining numbers in the same line
* Inner loop continues to next iteration
</details>

<h6><b> Example 3 Continue in Outer Loop </b></h6>
<details>
<summary>Explanation Example 3 </summary>

* Outer loop i runs 1 to 5
* When i == 3, continue skips entire iteration of outer loop
* Inner loop does not execute for i == 3
* Loop continues with i = 4
# Example 1 : Simple Loop
for i in range(1, 6):
    if i == 4:
        print("loop skips")
        continue
    print(i, end=" ")

# Example 2 : Nested Loop
for i in range(1, 6):
    for j in range(1, 4):
        if j == 2:
            print("loop skips")
            continue
        print(j, end=" ")
    print()

# Example 3 Continue in Outer Loop 
for i in range(1, 6):
    if i == 3:
        print("loop skips")
        continue
    for j in range(1, 4):
        print(i, end=" ")
    print()

<h5> Pass Statement<h5>
<details>
<summary>show more</summary>

* `pass` is a **null statement** in Python  
* It is used when a statement is **required syntactically**, but **no action is needed**  
* When `pass` is executed, **nothing happens**
</details>

<h6> <b> Example 1 :Program to print odd numbers from 1 to 5 </b></h6>
<details>
    <summary>Explanation Example 1</summary>

* Loop runs from 1 to 5
* Even numbers satisfy the if condition → pass does nothing
* Odd numbers go to else → printed
* Program continues without error
</details>

# Example 1 :Program to print odd numbers from 1 to 5 
for i in range(1, 6):
    if i % 2 == 0:
        pass
    else:
        print(i)

#### Program to Find Two Numbers Whose Sum Equals the Target
<details>
    <summary>Explanation soln:1</summary>
    
* A list `num` contains a set of numbers  
* `target` stores the required sum  
* Two **nested for loops** are used to check all possible pairs  
* The outer loop selects the first number  
* The inner loop selects the next number  
* If the sum of two numbers equals the target, their **indices are printed**  
* If not, `"No Match"` is displayed  
</details>

<details>
    <summary>Explanation soln:2</summary>

* Program checks **all possible pairs**  
* Prints `"No Match"` whenever the sum does not match  
* Even after finding the correct pair, loops continue  
* Results in **multiple "No Match" outputs**
</details>

<details>
    
<summary> Difference Between Two Programs </summary>

| Feature | With break | Without break |
|------|------------|---------------|
| Loop execution | Stops early | Runs fully |
| Efficiency | More efficient | Less efficient |
| Output | Only correct indices | Many "No Match" |
| Use case | Best approach | For learning purpose |



# solution1:Program to Find Two Numbers Whose Sum Equals the Target
num=[2,7,11,15]
target=78
for i in range(len(num)):
    for j in range(i+1,len(num)):
        if num[i]+num[j]==target:
            print(i,j)
        else:
            print(" No Match")
#solution 2: Program to Find Two Numbers Whose Sum Equals the Target
num=[2,7,11,15]
target=9
for i in range(len(num)):
    for j in range(i+1,len(num)):
        if num[i]+num[j]==target:
            print(i,j)
        break
## Data Structures – Introduction
<details>
    <summary> show more</summary>

* A **Data Structure (DS)** is a way of **organizing, storing, and managing data**  
* It helps in **efficient access, modification, and processing** of data  
* Choosing the correct data structure **improves program performance**

##### Why Data Structures are Important?

* Efficient use of **memory**  
* Faster **data access and manipulation**  
* Helps in writing **optimized and structured programs**  
* Required for **large data handling**

#### Types of Data Structures

##### 1. Primitive Data Structures
* Store **single value**
* Built-in data types

Examples:
- int  
- float  
- char  
- bool  

##### 2. Non-Primitive Data Structures
• Store **multiple values**
• Can be **linear or non-linear**

#### Classification of Data Structures

###### A. Linear Data Structures
• Data elements are arranged **sequentially**
• Easy to traverse

Examples:
- String  
- List / Array  
- Tuple  
- Stack  
- Queue  


###### B. Non-Linear Data Structures
• Data elements are arranged **hierarchically**
• More complex structure

Examples:
- Tree  
- Graph  
- Set  
- Dictionary  


###### Data Structures in Python

Python provides built-in data structures:

| Data Structure | Example |
|---------------|--------|
| String | "Python" |
| List | [1, 2, 3] |
| Tuple | (1, 2, 3) |
| Dictionary | {"a": 1} |
| Set | {1, 2, 3} |

</details>

<h3>String</h3>
<details>
    <summary>show more</summary>

* A **string** in Python is a sequence of characters enclosed within single quotes (`' '`) or double quotes (`" "`).  
* Strings can contain letters, numbers, symbols, and spaces.  
* Python does not have a separate character data type, so even a single character is treated as a string.

<u><h5> Creating a String</h5></u>
* Strings are created by assigning text to a variable using quotes.  
* Both single and double quotes work in the same way.

Example:
- `'Python'`
- `"Python"`

##### <u> Multi-line Strings</u>

* Multi-line strings are used when text spans across multiple lines.  
* They are created using triple quotes (`''' '''` or `""" """`).  
* Line breaks are preserved automatically.

##### <u> Accessing Characters in a String </u>

* Each character in a string has an index number.  
* Indexing starts from **0** for the first character.  
* Negative indexing starts from **-1** for the last character.

Example:
- `s[0]` gives first character  
- `s[-1]` gives last character  

##### <u> String Slicing</u>
* Slicing is used to extract a part of a string.  
* The syntax is `string[start:end]`.  
* The start index is included, but the end index is excluded.
<u>String Slicing step</u>
* The syntax is `string[start:end:step]`

Example:
- `s[1:4]` extracts characters from index 1 to 3  
- `s[::-1]` reverses the string
- `s[1:3:-1]` step
##### <u> String Iteration</u>
* Strings are iterable, meaning we can loop through each character using a `for` loop.  
* Each iteration accesses one character at a time.

##### <u> String Immutability </u>
* Strings are **immutable**, which means they cannot be changed after creation.  
* We cannot modify a character directly.  
* To change a string, a new string must be created using slicing or methods.

##### <u> Deleting a String</u>
* Individual characters in a string cannot be deleted.  
* However, the entire string variable can be deleted using the `del` keyword.  
* After deletion, accessing the variable causes an error.

##### <u> Updating a String</u>
* Updating a string means creating a new string using:
  - Concatenation
  - Slicing
  - String methods like `replace()`

* The original string remains unchanged.

##### <u> Common String Methods </u>
Python provides many built-in string methods:
- `len()` – returns length of string  
- `upper()` – converts to uppercase  
- `lower()` – converts to lowercase  
- `strip()` – removes extra spaces  
- `replace()` – replaces part of string  

##### <u>String Concatenation and Repetition</u>
* Strings can be joined using the `+` operator.  
* Strings can be repeated using the `*` operator.

##### <u> String Formatting</u>
* String formatting allows inserting variables into strings.
* Python supports:
- **f-strings** (simplest method)
- **format() method**
 
##### <u> String Membership Testing </u>
* The `in` keyword checks whether a substring exists inside a string.  
* It returns `True` or `False`.

# Creating a String
s1 = 'REVA' # single quote
s2 = "Re v a" # double quote
print(s1)
print(s2)
# Multi-line Strings
s = """I am Learning
Python String"""
print(s)

s = '''I'm a
vv'''
print(s)
#Accessing Characters in a String 
# Example (Positive Index)
s = "Python -py thon"
print(s[0]) # first character
print(s[4]) # fifth character

# Example (Negative Index)
print(s[-10])
print(s[-5])
# String Slicing
s = "String Slicing"
print(s[1:4])
print(s[:3])
print(s[3:])
print(s[::-1])

#step
print(s[1:9:2])
# String Iteration
s = "Python"
for ch in s:
    print(ch)



# String Immutability
s = "python"
s = "P" + s[1:]
print(s)
## Deleting a String
s = "Python"
del s
# Updating a String
s = "hello v"
s1 = "H" + s[1:]
s2 = s.replace("v", "Python")
print(s1)
print(s2)
#  Common String Methods
s = "Hello World"
print(len(s))
print(s.upper())
print(s.lower())
print(s.strip())
print(s.replace("World", "awesome"))
print(s.replace("Wor", "awesome")) # using letter

s1 = "Hello"
s2 = "World"
print(s1 + " " + s2)

print(s * 3)

## Formatting Strings
### Using f-string
name = "Alice"
age = 22
print(f"Name: {name}, Age: {age}")
# Using format()
s = "My name is {} and I am {} years old.".format("abc", 23)
print(s)

## String Membership Testing
s = "Hello World"
print("Hello" in s)
print("hello" in s)
##### Common String Methods in Python

<details>
    <summary>show more</summary>

###### <u> count()</u>
*  Returns the **number of occurrences** of a substring in a string  
###### <u> index()</u>
* Returns the **index position** of the first occurrence of a substring  
* Raises **error** if substring is not found  
###### <u> capitalize()</u>
* Converts the **first character** of the string to uppercase  
* Rest of the string becomes lowercase
###### <u> find()</u>
* Returns the **index position** of a substring  
* Returns **-1** if substring is not found 
###### <u> split()</u>
* Splits a string into a **list of words**  
* Default separator is **space**
###### <u> strip()</u>
* Removes **leading and trailing spaces**  

</details>
<details>
    

##### Difference: index() vs find()

| Method | If substring not found |
|------|----------------|
| index() | Gives Error |
| find() | Returns -1 |
</details>

s = "hello world"
print(s.count("l"))
print(s.index("w"))
print(s.capitalize())
print(s.find("o"))
print(s.find("z"))
print(s.split())
print(s.strip())
<h3>List</h3>
<details>
    <summary>show more</summary>

* A **list** is an ordered collection of elements
* Lists are **mutable** (can be changed)  
* Elements in a list **need not be of the same data type**  
* Lists are similar to **arrays** in other programming languages  

##### Features of Python Lists
* Ordered (elements have a fixed position)  
* Allows duplicate values  
* Can store **mixed data types**  
* Dynamic in size  

##### <u>Creating a List</u>
* A list is created using **square brackets [ ]**.

##### <u>Indexing in List</u>
* Index starts from **0**  
* Last index is **N-1** (for N elements)  
* Negative indexing starts from **-1**

##### <u>Multi-Dimensional List</u>
* A list inside another list is called a **nested list**

List = [1, 2, 3, "AbcDe", 2.3]
print(List)
List2 = [['Abcd', 'Def'], ['lms',3]]
print(List2)
print(List[0]) # first element
print(List[2]) # third element
print(List[-1]) # last element
print(List[-3]) # third element from end
<h3>Tuple</h3>
<details>
    <summary>show more</summary>

* A <b>tuple</b> is an ordered collection of elements  
* Tuples are <b>immutable</b> (cannot be changed after creation)  
* Elements in a tuple <b>can be of different data types</b>  
* Tuples are similar to lists but are <b>read-only</b>  

##### Features of Python Tuples
* Ordered (elements have a fixed position)  
* Allows duplicate values  
* Can store <b>mixed data types</b>  
* Faster than lists  
* Immutable in nature  

##### <u>Creating a Tuple</u>
* A tuple is created using <b>parentheses ( )</b>  
* Single element tuple must contain a comma  

##### <u>Indexing in Tuple</u>
* Index starts from <b>0</b>  
* Last index is <b>N-1</b> (for N elements)  
* Negative indexing starts from <b>-1</b>  

##### <u>Nested Tuple</u>
* A tuple can contain another tuple inside it  

##### <u>Tuple Unpacking</u>
* Assigning tuple elements to multiple variables  
* <b>*</b> operator can be used to collect multiple values  

##### <u> Deleting a Tuple </u>
```python
tup = (0, 1, 2, 3, 4)
del tup
print(tup)
```
Output
NameError: name 'tup' is not defined

</details>
<h3>Tuple Unpacking with Asterisk (*)</h3>
<details>
    <summary>show more</summary>
Tuple Unpacking with Asterisk (*) Explanation:
a → first element
c → last element
*b → remaining elements stored as a list
</details>


#Create tuple
# Empty tuple
tup = ()
print(tup)

# Tuple using strings
tup = ('Python', 'For')
print(tup)

# Tuple from list
li = [1, 2, 4, 5, 6]
print(tuple(li))

# Tuple using tuple() function
tup = tuple('Python')
print(tup)

#Nested Tuple
tup1 = (0, 1, 2, 3)
tup2 = ('Python', 'Hello')
tup3 = (tup1, tup2)
print("Nested :",tup3)

#Tuple Repetition
tup = ('Python',) * 3
print("Repetition : ",tup)

#Indexing Tuple
tup = tuple("Python")
print("Indexing : ",tup[0])

#Slicing Tuple
print("Remove first element : ",tup[1:])     # Remove first element
print("Reverse tuple : ",tup[::-1])   # Reverse tuple
print("Range slicing : ",tup[4:9])    # Range slicing
print(tup[1:4])
print(tup[:3])

#Tuple Unpacking
tup4 = ("PYTHON", "vv", "python")
a, b, c = tup4
print(a)
print(b)
print(c)

#Concatenation of Tuples
tup5 = tup1 + tup2
print("Concatenation : ",tup5)

#Tuple Unpacking with Asterisk (*)
tup = (1, 2, 3, 4, 5,6,7,8,9)
a, *b, c = tup
print(a)
print(b)
print(c)


<h3>Dictionary</h3>
<details>
    <summary>show more</summary>

* A <b>dictionary</b> stores data in <b>key : value</b> pairs  
* Keys must be <b>unique</b> and <b>immutable</b>  
* Values can be of <b>any data type</b> and can be duplicated  
* Keys are <b>case-sensitive</b>  
* Dictionaries internally use <b>hashing</b>    

##### Features of Python Dictionary
* Stores data as <b>key : value</b> pairs  
* Fast access (search, insert, delete in constant time)  
* Keys cannot be repeated  
* Values can be changed   

##### <u>Creating a Dictionary</u>
* Dictionary is created using <b>curly braces { }</b>  
* Key and value are separated by <b>:</b>  
* Elements are separated by <b>commas</b>  

##### <u>Accessing Dictionary Items</u>
* Values can be accessed using <b>keys</b>  
* Access methods:
  * Square brackets <b>[ ]</b>
  * <b>get()</b> method  

##### <u>Adding and Updating Items</u>
* New key-value pairs can be added  
* Existing values can be updated using keys  

##### <u>Removing Dictionary Items</u>
* <b>del</b> – removes item using key  
* <b>pop()</b> – removes and returns value  
* <b>popitem()</b> – removes last inserted item  
* <b>clear()</b> – removes all items  

##### <u>Iterating Through Dictionary</u>
* Iterate using:
  * <b>keys()</b> – for keys  
  * <b>values()</b> – for values  
  * <b>items()</b> – for key-value pairs  

</details>

# Creating a dictionary
stu = {
    "name": "Rahul",
    "age": 20,
    "course": "Python"
}

print("Dictionary:")
print(stu)

# Accessing values
print("\nAccessing values:")
print("Name:", stu["name"])
print("Age:", stu.get("age"))

# Adding a new key-value pair
stu["college"] = "REVA"
print("\nAfter Adding college:")
print(stu)

# Updating an existing value
stu["age"] = 21
print("\nAfter Updating age:")
print(stu)

# Removing an item using pop()
removed_value = stu.pop("course")
print("\nRemoved Value:", removed_value)
print("After Removing course:")
print(stu)

# Iterating through dictionary
print("\nIterating through Dictionary:")
for key, value in stu.items():
    print(key, ":", value)

# Clearing the dictionary
stu.clear()
print("\nAfter Clearing Dictionary:")
print(stu)

<h2>Set</h2>

<details>
<summary>Show more</summary>

> A **Set** in Python is an **unordered**, **unindexed**, and **mutable** collection of **unique elements**.

### Characteristics of Set
- Stores unique elements only
- Unordered collection (order may change)
- Mutable (elements can be added or removed)
- Does not support indexing
- Can store different data types
- Implemented using hash tables internally

<h5><U>Creating a Set</U></h5>


Python provides two ways to create a set:
- Using curly braces `{ }`
- Using the built-in `set()` function


<h5><U>Unordered and Unindexed Nature</U></h5>

- The order of elements in a set is not preserved
- Indexing is not supported in sets


<h5><U>Adding Elements to a Set<U></h5>

- `add()` → adds one element
- `update()` → adds multiple elements

<h5><U>Accessing Elements in a Set</U></h5>

- Use `for` loop to access elements
- Use `in` keyword to check membership

<h5><U>Removing Elements from a Set</U></h5>

- `remove()` → removes element (error if not present)
- `discard()` → removes element (no error)
- `pop()` → removes random element
- `clear()` → removes all elements

<h5><U>Frozen Set</U></h5>

A **frozenset** is an immutable set. Once created, elements cannot be added or removed.

<h5><U>Maximum and Minimum Element in Set</U></h5>

Python provides built-in functions `min()` and `max()` to find minimum and maximum elements in a set.


<h5><U>Common Python Set Methods</U></h5>

| Method | Description |
|------|-------------|
| add() | Adds an element |
| remove() | Removes an element |
| discard() | Removes without error |
| pop() | Removes random element |
| clear() | Removes all elements |
| union() | Returns union of sets |
| intersection() | Returns common elements |

# Creating sets
set1 = {1, 2, 3, 4}
print(set1)

set2 = set()
print(set2)

set3 = set("PYTHONpython")
print(set3)

set4 = set(["PYT", "ON", "python"])
print(set4)

# Unordered and unindexed
set5 = {3, 1, 4, 1, 5, 9, 2}
print(set5)

# Adding elements
set6 = {1, 2, 3}
set6.add(4)
set6.update([5, 6])
print(set6)

# Accessing elements
set7 = {"PYT", "ON", "python"}
for item in set7:
    print(item)
print("PYT" in set7)

# Removing elements
set8 = {1, 2, 3, 4, 5}
set8.remove(3)
set8.discard(10)
print("Popped:", set8.pop())
print(set8)
set8.clear()
print(set8)

# Frozen set
fset = frozenset([1, 2, 3, 4, 5])
print(fset)

# Min and Max
s = {4, 12, 10, 9, 13}
print("Minimum:", min(s))
print("Maximum:", max(s))

<h2>Functions</h2>

<details>
<summary>Show more</summary>

> A **function** is a block of reusable code that runs **only when it is called**.

- Avoids code repetition
- Improves code readability
- Makes program modular
- A function can return data as a result


<h5>Syntax of a Function</h5>

> In Python, a function is defined using the **def** keyword.

##### <B> General Syntax </B>

```python
def function_name(parameters):
    statement(s)
 ```
<U><B>Explanation</U></B>
<details>
<summary>Show more</summary>

* def → Keyword used to define a function
* function_name → Name of the function
* parameters → Values passed to the function (optional)
* statement(s) → Block of code executed 
</details> 


<h5><U>Calling a Function</U></h5>

- A function is executed by calling its name followed by parentheses
- The same function can be called multiple times

</details>

# Creating a function
def my_function():
    print("Hello from a function")

# Calling the function
my_function()

# Calling the function multiple times
my_function()
my_function()
my_function()

<h4>EXAMPLE :Factorial of a Number Using Function</h4>
<details>
<summary>Show more</summary>

| Method | Technique | Explanation |
|------|----------|-------------|
| Method 1 | Function + Loop | Uses `for` loop to multiply numbers from 1 to n |
| Method 2 | math Module | Uses built-in `math.factorial()` |
| Method 3 | Recursion | Function calls itself until base condition |

</details>

<h5>Method 1: Factorial Using Function and Loop</h5>

<details>
<summary>Show more</summary>

**Steps:**
* Function `fac(n)` is defined.
* Variable `fact` is initialized to 1.
* Loop runs from 1 to n.
* Each number is multiplied with `fact`.
* Final value is returned.

</details>

<h5>Method 2: Factorial Using math Module</h5>

<details>
<summary>Show more</summary>

**Steps:**
* Import `math` module.
* Read input from user.
* Use `math.factorial()` to calculate factorial.

</details>


<h5>Method 3: Factorial Using Recursion</h5>

<details>
<summary>Show more</summary>

**Steps:**
* Function calls itself.
* Base condition: if n == 0 return 1.
* Recursive call multiplies n with factorial of (n-1).
* Final result is returned.

</details>


# Method 1: Factorial using function and loop
def fac(n):
    fact = 1
    for i in range(1, n + 1):
        fact *= i
    return fact

num = int(input("Enter a number: "))
print("Factorial using loop:", fac(num))


# Method 2: Factorial using math module
import math
fact = int(input("Enter a number: "))
print("Factorial using math module:", math.factorial(fact))


# Method 3: Factorial using recursion
def fact_rec(n):
    if n == 0:
        return 1
    else:
        return n * fact_rec(n - 1)

num = int(input("Enter a number: "))
print("Factorial using loop:", fac(num))



<h3>Ways to Write a Function in Python</h3>

<details>
<summary>Show more</summary>

> In Python, a function can be written in **four different ways** based on:
- Whether it **accepts arguments**
- Whether it **returns a value**

1. With arguments and with return type  
2. With arguments and without return type  
3. Without arguments and with return type  
4. Without arguments and without return type



<h5>1. With Arguments and With Return Type (+ , +)</h5>

<details>
<summary>Show more</summary>

- Function **takes input through arguments**
- Function **returns the result**
- Most efficient and reusable method

**Explanation:**
1. Values are passed to the function.
2. Addition is performed inside the function.
3. Result is returned using `return`.
4. Returned value is printed outside the function.

</details>


<h5>2. With Arguments and Without Return Type (+ , -)</h5>

<details>
<summary>Show more</summary>

- Function **takes arguments**
- Function **does not return value**
- Output is printed inside the function

**Explanation:**
1. Values are passed to the function.
2. Addition is performed.
3. Result is printed directly.

</details>


<h5>3. Without Arguments and With Return Type (- , +)</h5>

<details>
<summary>Show more</summary>

- Function **does not take arguments**
- Input is taken inside the function
- Result is returned

**Explanation:**
1. Input is taken inside the function.
2. Addition is performed.
3. Result is returned.
4. Returned value is printed outside.

</details>

<h5>4. Without Arguments and Without Return Type (- , -)</h5>

<details>
<summary>Show more</summary>

- Function **does not take arguments**
- Function **does not return value**
- Input and output handled inside the function

**Explanation:**
1. Input is taken inside the function.
2. Addition is performed.
3. Result is printed inside the function.

</details>


<h5>Difference Between All Four Ways</h5>

| Method | Arguments | Return Type | Input Location | Output Location | Reusability |
|------|----------|-------------|----------------|-----------------|-------------|
| Way 1 | Yes | Yes | Outside | Outside | High |
| Way 2 | Yes | No | Outside | Inside | Medium |
| Way 3 | No | Yes | Inside | Outside | Medium |
| Way 4 | No | No | Inside | Inside | Low |

</details>

# 1. With arguments and with return type (+,+)
def sum(n1, n2):
    s = n1 + n2
    return s

x = float(input("ENTER NUM1: "))
y = float(input("ENTER NUM2: "))
print(sum(x, y))


# 2. With arguments and without return type (+,-)
def sum(n1, n2):
    s = n1 + n2
    print(s)

x = float(input("ENTER NUM1: "))
y = float(input("ENTER NUM2: "))
sum(x, y)


# 3. Without arguments and with return type (-,+)
def sum():
    x = float(input("ENTER NUM1: "))
    y = float(input("ENTER NUM2: "))
    s = x + y
    return s

print(sum())


# 4. Without arguments and without return type (-,-)
def sum():
    x = float(input("ENTER NUM1: "))
    y = float(input("ENTER NUM2: "))
    s = x + y
    print(s)

sum()

<h3>Types of Functions in Python</h3>

<details>
<summary>Show more</summary>

Python functions are mainly classified into two types:

<h5>1. Pre-defined Function</h5>

A pre-defined function is a function that is already available in Python.
These functions are built-in and provided by Python itself.
The user can use these functions directly but **cannot modify or change their definition**.

<b>Examples:</b> print(), len(), type()


<h5>2. User-defined Function</h5>

A user-defined function is a function created by the programmer.
The user writes the function according to their requirement.
These functions can be modified, reused, and customized.

<b>Example:</b> add(), sum()


<h5>Difference Between Pre-defined and User-defined Functions</h5>

| Feature | Pre-defined Function | User-defined Function |
|-------|---------------------|----------------------|
| Definition | Already defined in Python | Defined by user |
| Modification | Cannot be changed | Can be changed |
| Examples | print(), len() | add(), sum() |

</details>

# Pre-defined function example
text = "Python"
print(len(text))

# User-defined function example
def add(a, b):
    return a + b

print(add(10, 20))

<h3>Anonymous Function (Lambda Function)</h3>

<details>
<summary>Show more</summary>

An anonymous function is a function without a name.  
It is defined using the keyword <b>lambda</b>.

<b>Syntax:</b>
```
lambda arguments : expression
```
<h3>Scope of Variable</h3>

<details>
<summary>Show more</summary>
<b>Scope</b> refers to the area of a program where a variable can be accessed.

There are two main types of variable scope in Python:
1. Local Variable
2. Global Variable
<h5>1. Local Variable</h5>

- A variable declared <b>inside a function</b>
- Accessible only within that function
- Created when the function is called
- Destroyed when the function ends

<h5>2. Global Variable</h5>

- A variable declared <b>outside a function</b>
- Accessible throughout the program
- Can be used inside functions (read-only by default)


def my_function():
    x = 10   # Local variable
    print("Inside function:", x)

my_function()

# print(x)  # Error: x is not defined outside the function
y = 20   # Global variable

def my_function():
    print("Inside function:", y)

my_function()
print("Outside function:", y)

<h3>PROGRAM : Text Cleaning and Word Processing in Python</h3>
<details>
<summary>Show more</summary>
<b>Program Objective:</b>  
This program processes a text message by removing punctuation, converting it to lowercase, splitting it into words, and analyzing the words.


1. Import the `string` module  
   - Used to access punctuation symbols.

2. Store text in a variable  
   - The given feedback text is stored in a variable.

3. Remove punctuation  
   - `translate()` and `string.punctuation` remove symbols like !, @, #, etc.

4. Convert text to lowercase  
   - Ensures uniformity (e.g., "BUY" and "buy" become the same).

5. Split text into words  
   - Converts the sentence into a list of words.

6. Count total words  
   - `len()` counts how many words are present.

7. Remove duplicate words  
   - `set()` removes repeated words.

8. Sort unique words  
   - `sorted()` arranges words in alphabetical order.

# Text Cleaning and Word Processing in Python
import string

feedback = "Awesome PRODUCT!!! Loved it... Will BUY again & again!!!"

# Remove punctuation
clear_text = feedback.translate(str.maketrans("", "", string.punctuation))
print(clear_text)

# Convert text to lowercase
lower_case = clear_text.lower()
print(lower_case)

# Split text into words
word_list = lower_case.split()
print(word_list)

# Count & sort
print(len(word_list))            # Total number of words
print(set(word_list))            # Unique words
print(sorted(set(word_list)))    # Sorted unique words

PROGRAM : <h3>Hospital OPD Queue Management System (Using Queue)</h3>
<details>
<summary>Show more</summary>
<b>Program Objective:</b>  
This program simulates a Hospital OPD queue system where patients are added, removed after consultation, and displayed in order.


<b>Step-by-Step Explanation:</b>

1. Create an empty list `queue`
   - Stores patient names in order of arrival.

2. Set maximum queue size
   - `MAX_QUEUE = 10` limits the number of patients.

3. Display menu repeatedly
   - `while True` keeps the program running until exit.

4. Add New Patient
   - Checks if queue is full
   - Adds patient name using `append()`.

5. Remove Patient After Consultation
   - Removes first patient using `pop(0)`
   - Follows FIFO principle.

6. Show Current Queue
   - Displays all patients waiting in the queue.

7. Exit Option
   - Stops the program using `break`.

8. Invalid Choice Handling
   - Displays error message for wrong input.

#Hospital OPD Queue Management System (Using Queue)
queue = []
MAX_QUEUE = 10

while True:
    print("\nHospital OPD Queue System")
    print("1. Add New Patient")
    print("2. Remove Patient After Consultation")
    print("3. Show Current Queue")
    print("4. Exit")
    
    choice = input("Enter your choice (1-4): ")

    if choice == '1':
        if len(queue) >= MAX_QUEUE:
            print("Queue is full! Cannot add more patients.")
        else:
            patient_name = input("Enter patient name: ")
            queue.append(patient_name)
            print(f"{patient_name} added to the queue.")
            
    elif choice == '2':
        if queue:
            removed = queue.pop(0)
            print(f"{removed} has been removed after consultation.")
        else:
            print("Queue is empty! No patient to remove.")
            
    elif choice == '3':
        if queue:
            print("Current Queue:", queue)
        else:
            print("Queue is empty!")
            
    elif choice == '4':
        print("Exiting the system...")
        break
        
    else:
        print("Invalid choice! Please enter 1-4.")

## Smart Salary Processing System Problem Scenario 
<details><summary>show Q </summary>
A multinational company uses an automated payroll system to calculate monthly net salaries. Each employee record contains basic salary, years of experience, and performance rating. 
 
Business Rules

- Experience ≥ 5 years → 10% bonus 
- Performance rating ≥ 4 → additional 5% bonus 
- Salary > ₹80,000 → 20% tax 
- Otherwise → 10% tax 
Task 
Write a Python function to compute and display the net salary for each employee

Sample Input 
 
Employees: 
Ravi, 90000, 6, 4 
Anita, 60000, 3, 5 
Suresh, 85000, 8, 3 
 
Sample Output 
 
Employee: Ravi   | Net Salary: ₹77400 
Employee: Anita  | Net Salary: ₹56700 
Employee: Suresh | Net Salary: ₹68850
</details>
# IA1 Q 1 Smart Salary Processing System Problem Scenario
def salary(name, basic_salary, experience, rating):
    salary=basic_salary
    
    # experience
    if experience>=5:
        salary+=basic_salary*0.10
    
    # rating
    if rating>=4:
        salary+=basic_salary*0.05
    
    # Tax deduction
    if salary>80000:
        tax=salary*0.20
    else:
        tax=salary*0.10
    
    net_salary=salary-tax
    
    print(f"Employee: {name} | Net Salary: ₹{int(net_salary)}")


# Input
employees = [
    ("Ravi", 90000, 6, 4),
    ("Anita", 60000, 3, 5),
    ("Suresh", 85000, 8, 3)
]

# Processing each employee
for emp in employees:
    salary(emp[0], emp[1], emp[2], emp[3])

## Smart Electricity Billing Automation System Problem Scenario 
<details><summary>show Q</summary>


    A power distribution company is developing an automated electricity billing system to calculate monthly bills for its customers. The system records the total number of electricity units consumed by a household during a billing cycle and computes the bill amount based on slab-wise tariff rules. As an Automation Engineer, you are required to design a Python program that calculates the total electricity bill automatically using conditional logic. 
 
Billing Rules: 
 
Unit Consumption Charge 
First 100 units No charge 
Next 100 units (101–200) ₹5 per unit 
Above 200 units ₹10 per unit 
 
Task: 
Write a Python program that: 
1. Accepts the total number of units consumed from the user. 
2. Applies slab-wise billing rules. 
3. Calculates and displays the final electricity bill amount.
</details>
#IA1 Q 3  Electricity Billing Automation System

# input
units=int(input("Enter total units consumed: "))

# Calculate bill 
if units<=100:
    bill=0
elif units<=200:
    bill=(units-100)*5
else:
    bill=(100*5)+(units-200)*10

# Display output
print("\nElectricity Bill Summary:")
print("Units Consumed:", units)
print("Total Bill Amount: ₹{}".format(bill))

## Extracting the First Digit of a Number Problem Scenario
<details><summary>Show Q</summary>
In many data validation and preprocessing systems, it is often necessary to extract specific digits from numerical identifiers such as transaction IDs, customer numbers, or sensor readings. As part of a preprocessing module, you are required to determine the first (most significant) digit of a given positive integer. 
 
Task 
Given a positive integer n, write a program to find and return the first digit of the number. 
 
Sample Input: 
989 
 
Sample Output: 
9
</details>
#IA1 Q 5 Extracting the First Digit of a Number Problem Scenario 
# input
n=int(input("Enter a positive integer: "))

# Find first digit
while n>=10:
    n=n//10

# Display result
print("First Digit:", n)

# File Handling – Introduction
<details>
<summary>Show more</summary>
    
- **File Handling** is a way of **storing data permanently on secondary storage**
- **File Handling** in Python refers to the processing of **createing, reading, writing, updating, and deleting files** using built-in functions.
- Helps in **data persistence**, even after program execution ends



### Why File Handling is Important?
<details>
<summary>Show more</summary>
    
- Stores data **permanently**
- Avoids **data loss** after program termination
- Handles **large amounts of data efficiently**
- Useful for **real-world applications** like databases, logs, reports 

</details>

### Real-Time Applications
<details>
<summary>Show more</summary>
    
- Saving user registration data
- Reading machine learning datasets
- Log

</details>

### Types of Files
<details>
<summary>Show more</summary>
    
#### 1. Text Files
<details>
<summary>Show more</summary>

**Definition:**
Text files are files that contain human-readable characters encoded using ASCII or Unicode.
Each character is stored as a byte representing letters, numbers, and special symbols.

**Features:**
- Can be opened and read using a normal text editor
- Stored in readable form
- Uses .txt, .log, .md extensions

**Examples:**
.txt, .log, .md
</details>

#### 2. Binary Files
<details>
<summary>Show more</summary>

**Definition:**
Binary files store data in binary format (0s and 1s).
They are not human-readable and require special software or programs to read and interpret them.

**Features:**
- Faster to read/write than text files
- Stores images, audio, video, documents
- Data is machine-readable

**Examples:**
.jpg, .png, .pdf, .mp3, .exe
</details>

#### 3. CSV Files (Comma-Separated Values)
<details>
<summary>Show more</summary>

**Definition:**
CSV files are specialized text files where data is stored in tabular format.
Each row is separated by a newline, and values in a row are separated by commas (or other delimiters).

**Features:**
- Easy to read and write
- Commonly used for data exchange
- Can be opened in Excel and databases

**Examples:**
.csv
</details>

#### Difference Between Text Files, Binary Files, and CSV Files
<details>
<summary>Show more</summary>

| **Parameter**           | **Text Files**                              | **Binary Files**                                    | **CSV Files**                                |
| ----------------------- | ------------------------------------------- | --------------------------------------------------- | -------------------------------------------- |
| **Readability**         | Human-readable (ASCII / Unicode)            | Not human-readable (machine format)                 | Human-readable (structured text)             |
| **Data Representation** | Characters, strings, numbers stored as text | Raw bytes (images, executables, serialized objects) | Tabular data with comma-separated values     |
| **Storage Efficiency**  | Less efficient (larger file size)           | Highly efficient (compact storage)                  | Moderate efficiency (due to delimiters)      |
| **Editing / Viewing**   | Any text editor (Notepad, VS Code)          | Requires specialized tools or programs              | Text editors or spreadsheet software (Excel) |
| **Data Integrity**      | May lose formatting across platforms        | Preserves exact data structure                      | Depends on consistent delimiters and format  |
| **Examples**            | `.txt`, `.log`, `.md`                       | `.jpg`, `.png`, `.pdf`, `.exe`                      | `.csv`                                       |
</details>
</details>

### Types Path of Files
<details>
<summary>Show more</summary>

#### 1. Absolute Path
<details>
<summary>Show more</summary>
    
**Definition:**  
An **absolute path** specifies the complete location of a file starting from the **root directory** of the system.

**Example:** C:\Users\paramesh\Desktop\Delete\file handling.txt


**Characteristics:**
- Starts from the root directory
- Directory independent
- Longer path length
- Harder to type
- More reliable in scripts
</details>

#### 2. Relative Path
<details>
<summary>Show more</summary>

**Definition:**  
A **relative path** specifies the location of a file **relative to the current working directory**.

**Example:**
Delete\file handling.txt

**Characteristics:**
- Depends on the current working directory
- Shorter path length
- Easier to type
- Less reliable in scripts

</details>

#### Difference Between Absolute and Relative Path
<details>
<summary>Show more</summary>
    
| Parameter | Absolute Path | Relative Path |
|--------|---------------|---------------|
| Definition | Complete path from root directory | Path relative to current directory |
| Path Length | Longer | Shorter |
| Directory Dependence | Independent | Dependent |
| Ease of Typing | Harder | Easier |
| Reliability | Reliable in scripts | Unreliable if directory changes |
| Example | `C:\Users\paramesh\Desktop\Delete\file handling.txt` | `Delete\file handling.txt` |


</details>
</details>

### File Operations
<details>
<summary>Show more</summary>

- Create a file  
- Open a file  
- Read data  
- Write data  
- Append data  
- Close the file

#### File Operations using `open()` Function

**Definition**
The `open()` function is used to open a file and returns a **file object**.  
This file object is used to perform read, write, and append operations.

## Syntax
```

file = open("data.txt", "r")
```

### Explanation
- `"data.txt"` → Name of the file  
- `"r"` → Mode (read mode)  
- `file` → File object returned by `open()`

</details> 

### File Modes in Python
<details>
<summary>Show more</summary>
    

  
| Mode | Description |
|------|------------|
| `r` | Read mode |
| `w` | Write mode |
| `a` | Append mode |
| `r+` | Read & Write |
| `b` | Binary mode |
| `t` | Text mode |
</details>


#### Example Program (Create File)
<details> <summary>Show more</summary>

```
    file_name = open("file handling.txt", "x")
```
**Explanation:**

`open("file handling.txt", "x")`
- Opens a file named file handling.txt in exclusive creation mode.
- The "x" mode creates a new file.
- If the file already exists, it raises a FileExistsError.
- file_name
This is a file object that you can use to write to the file using methods like write().
`file_name.close()`
</details>


#### Example Program (Read File)
<details>
<summary>Show more</summary>

```python
file = open("data.txt", "r")
print(file.read())
file.close()
```


#### Explanation:

- `open("data.txt", "r")`  
  Opens the file **data.txt** in **read mode**.  
  The file must already exist.

- `file.read()`  
  Reads the **entire content** of the file as a string.

- `print()`  
  Displays the file content in the output.

- `file.close()`  
  Closes the file and releases system resources.

</details>



#### Example Program (Write File)
<details>
<summary>Show more</summary>

```python
file=open("data.txt","w")
file.write("hello world")
file.close()

```
#### Explanation:

- `open("data.txt", "w")`  
  Opens the file **data.txt** in **write mode** (`"w"`).  
  - If the file **does not exist**, Python creates it.  
  - If the file **already exists**, its content is **overwritten**.

- `file.write("hello world")`  
  Writes the string `"hello world"` into the file.  
  - Note: It **does not automatically add a new line**.

- `file.close()`  
  Closes the file and **saves all changes**, releasing system resources.
</details>


### Python File Reading Methods
<details>
<summary>Show more</summary>
    
#####  1. read()
**Usage:** Reads the entire file as a single string.

**Example:**
```
file = open("file handling.txt", "r")
content = file.read()
print(content)
file.close()
```
**Notes:**
- Reads everything at once.
- Good for small files, not efficient for very large files.

##### 2. readline()
**Usage:** Reads one line at a time from the file.

**Example:**
```
file = open("file handling.txt", "r")
line1 = file.readline()
line2 = file.readline()
print(line1)
print(line2)
file.close()
```
**Notes:**
- Each call reads the next line.
- Useful for line-by-line processing.

##### 3. readlines()
**Usage:** Reads all lines and returns a list of strings, where each string is a line.

**Example:**
```
file = open("file handling.txt", "r")
lines = file.readlines()
print(lines)
file.close()
```
**Notes:**
- Returns a list, e.g., ["Line1\n", "Line2\n"].
- Easier for iterating through lines using loops:

**Method	Returns	Reads**
read()	Single string	Entire file
readline()	Single line string	One line at a time
readlines()	List of strings	All lines
</details>

#### Program: Read or Reading File and Splitting Words
<details><summary>Show more</summary>
    
```
file_name = open("file handling.txt", "r")
anything = file_name.read()
for i in anything.split():
    print(i)
file_name.close()
```


**Explanation**
`open("file handling.txt", "r")`
Opens the file in read mode.

`file_name.read()`
Reads the entire content of the file and stores it in the variable anything.

`anything.split()`
Splits the text into individual words using spaces as separators.

`for i in anything.split():`
Loops through each word in the file.

`print(i)`
Prints one word per line.

`file_name.close()`
Closes the file to free memory and resources.
</details>

#### Program: Reading File Using readlines()
<details><summary>show more</summary>

```
file_name=open("file handling.txt","r")
for i in file_name.readlines():
    print(i,end="")
    file_name.close()
```
**Explanation**

`open("file handling.txt", "r")`

Opens the file in read mode.

`file_name.readlines()`

Reads all lines from the file and returns them as a list.

`for i in file_name.readlines():`

Goes through the file line by line.

`print(i, end="")`
Prints each line.
end="" prevents extra blank lines.

`file_name.close()`
Closes the file after reading is completed.
</details>


#### Display lines in a file which word "GPT" in it
<details><summary>Show more</summary>

```
f1=open("file handling.txt","r")
count=0
lines=f1.readlines()
for i in lines:
    if(i.count("GPT")>0):
        print(i)
f1.close()
```

**Explanation**

`f1 = open("file handling.txt", "r")`
- Opens the file in read mode.
- Allows reading text from the file

`lines = f1.readlines()`
- Reads all lines from the file.
- Stores them as a list of strings.

`for i in lines:`
- Loops through the file line by line.

`if i.count("GPT") > 0:`
- count("GPT") returns the number of times "GPT" appears.
- If greater than zero, the word exists in that line.

`print(i)`
- Prints only lines that contain "GPT".

  </details>
</details>
# Example Program (Create File)
file=open("file handling.txt","x")

file=open("file handling.txt","r")
file.read()

file=open("file handling.txt","r")
print(file.read())

# Example Program (Read File)
file = open("data.txt", "r")
print(file.read())
file.close()
# Example Program (Write File)
file=open("data.txt","w")
file.write("hello world")
file.close()
file=open("simple.txt","c")
file.close()
file=open("data.txt","a")
file.write("hello")
file.close()

# Example read in split
file_name=open("file handling.txt","r")
anything=file_name.read()
for i in anything.split():
    print(i)
file_name.close()
# Program: Reading File Using readlines()
file_name=open("file handling.txt","r")
for i in file_name.readlines():
    print(i,end="")
    file_name.close()
# Write a program to count the number of upper-case letters present in a text file

f1=open("file handling.txt","r")
line=f1.read()

upper=0
for i in line:
    if(i.isupper()==True):
        upper+=1
        print("total upper letter",upper)

#Display lines a file which word on "GPT" in it

f1=open("file handling.txt","r")
count=0
lines=f1.readlines()
for i in lines:
    if(i.count("GPT")>0):
        print(i)
f1.close()
## Write a function lines_count() that reads lines from a text file named 'zen txt and displays the lines that begin with any vowel. Assume the file contains the following text and already exists on the computer's disk:
#Write a function lines_count() that reads lines from a text file named 'zen txt and displays the lines that begin with any vowel. Assume the file contains the following text and already exists on the computer's disk:
def lines_count():
    with open("zen.txt", "w") as file:
        file.write("""Beautiful is better than ugly.
Explicit is better than implicit.
Simple is better than complex.
Complex is better than complicated.
""")

    with open("zen.txt", "r") as file:
        for line in file:
            line = line.strip()
            if line and line[0].lower() in ['a','e','i','o','u']:
                print(line)

lines_count()


## Write a Python function named feedback_analysis() to calculate and display the following information:

1. Total feedbacks stored in the file,

2. Count of positive feedbacks,

3. Count of negative feedbacks.
#Write a Python function named feedback_analysis() to calculate and display the following information:
with open("feedback.txt", "w") as f:
    f.write("""Positive: Ram excelled.
Negative: Maya struggled.
Positive: Ramesh performed well.
Negative: Alex needs improvement.""")
 
def feedback_analysis():
    total = positive = negative = 0
    with open("feedback.txt", "r") as f:
        for line in f:
            if line.strip():
                total += 1
                if line.startswith("Positive"):
                    positive += 1
                elif line.startswith("Negative"):
                    negative += 1
    print("Total:", total)
    print("Positive:", positive)
    print("Negative:", negative)
 
feedback_analysis()
## Exceptions in Python
<details> <summary>Show more</summary>

**Definition**
An exception is an error that occurs during program execution.

**Key Points**
- Errors that happen while the program is running
- Forces the program to display an error message
- Current process stops when an exception occurs
- Exception is passed to the calling process
- Continues passing until it is handled
- If not handled, the program crashes
- Exception is the base class for all exceptions in Python

### Common Exceptions in Python
<details> <summary>Show more</summary>

**An exception is an error that occurs during the execution of a program and interrupts the normal flow.** <br>
**1. ZeroDivisionError**

**Definition:-**
Occurs when a number is divided by zero.

**Example:**
```
a = 10
b = 0
print(a / b)
```
<br>

**2. NameError**

**Definition:-**
Occurs when a variable or function name is not defined (not found in local or global scope).

**Example:**
```
print(x)
```
<br>

**3. IndentationError**

**Definition:-**
Occurs when indentation (spaces/tabs) is incorrect.

**Example:**
```
if True:
print("Hello")
```
<br>

**4. IOError**

**Definition:-**
Occurs when an input/output operation fails (file not found, permission denied, etc.).

**Example:**
```
file = open("data.txt", "r")
```
<br>

**5. EOFError**

**Definition:-**
Occurs when the end of file is reached but input is still expected.

**Example:**
```
input()
```

<br>

**6. IndexError**

**Definition:-**
Occurs when an index is out of range.

**Example:**
```
a = [1, 2, 3]
print(a[5])
```

<br>

**7. ImportError**

**Definition:-**
Occurs when Python cannot find or load a module.

**Example:**
```
import abcdef
```

<br>

**8. ValueError**

**Definition:-**
Occurs when a function receives the correct type but an inappropriate value.

**Example:**
```
int("abc")
```
<br>

**9. KeyboardInterrupt**

**Definition:-**
Occurs when the user interrupts the program execution (Ctrl + C).

**Example:**
```
while True:
    pass
```
</details>

### Exception Handling
<details> <summary>Show more</summary>

- The try block lets you test a block of code for errors.
- The except block lets you handle the error.
- The else block lets you execute code when there is no error.
- The finally block lets you execute code, regardless of the result of the try- and except blocks.

#### Try Block

**Definition:-**
- The try block contains the code that may cause an exception (error).
- It must always be followed by at least one except block.

**Key Points**

- The try block contains risky code.
- If an error occurs in the try block, control is transferred to the except block.
- A try block cannot exist alone without an except or finally block.

**Syntax of Try–Except**
```python
try:
    # Run this code
except:
    # Run this code if an exception occurs
```

**Explanation**

try:
Executes the statements that may generate an exception.

except:
Executes only when an exception occurs in the try block.

**Example**
```python
try:
    a = 10
    b = 0
    print(a / b)
except:
    print("Error: Division by zero")
```
**Output**
Error: Division by zero
  


**Program : Basic try–except Block**
<details> <summary>Explanation</summary>

```python
try:
    a = 10
    b = 0
    print(a // b)
except:
    print("Input Invalid")
```

**Explanation**

- The try block contains code that may cause an error.
- Here, division by zero occurs (b = 0).
- Python raises a ZeroDivisionError.
- The except block catches the error and prints "Input Invalid".
</details>

**Program : Using Exception Class**
<details> <summary>Explanation</summary>

```python
try:
    a = int(input("enter the a : "))
    b = int(input("enter the b : "))
    print(a // b)
except Exception:
    print("Input Invalid")
```
**Explanation**
- User inputs values for a and b.
- Errors may occur due to:
- Invalid input (letters instead of numbers)
- Division by zero
- Exception is the base class of all exceptions.
- This except block catches any type of exception.
- Displays a general error message.

</details>

**Program : Using Exception as e**
<details> <summary>Explanation</summary>

```python
try:
    a = int(input("enter the a : "))
    b = int(input("enter the b : "))
    print(a // b)
except Exception as e:
    print(e)
```
**Explanation**

- Same as Program 2, but:
- The error message is stored in variable e.
- print(e) displays the actual system error message.
- Helps in debugging.



**Program: try with except (No finally)**
<details> <summary>Explanation</summary>

```python
    try:
    print("File Open")
    a = int(input("enter the a : "))
    b = int(input("enter the b : "))
    print(a // b)
    print("File Close")
except Exception as e:
    print(e)
```

**Explanation:**
- try block contains normal program statements.
- If no error occurs:
- "File Open" is printed
- Division result is printed
- "File Close" is printed
- If any exception occurs (e.g., divide by zero, invalid input):
- Control moves to except
- Error message is printed
- "File Close" will NOT execute because it is inside try
</details>
</details>

**Program: try–except with manual file closing**
<details> <summary>Explanation</summary>
    
```python
try:
    print("File Open")
    a = int(input("enter the a : "))
    b = int(input("enter the b : "))
    print(a // b)
    print("File Close")
except Exception as e:
    print(e)
    print("File Close")
```
**Explanation:**
- Ensures "File Close" executes in both:
- Normal execution
- Exception case
- But this approach is not recommended due to duplication

</details>

#### Finally Block 
<details> <summary>Show more</summary>
    
- The finally block is used with the try block.
- It contains code that must be executed whether an exception occurs or not.
- It is mainly used for cleanup operations such as:
- Closing files
- Releasing resources
- Closing database connections

**Syntax**
```python
try:
    # block of code
    # this may throw an exception
finally:
    # block of code
    # this will always be executed
```

**Program: try–except–finally**
<details> <summary>Explanation</summary>

```python
try:
    print("File Open")
    a = int(input("enter the a : "))
    b = int(input("enter the b : "))
    print(a // b)
except Exception as e:
    print(e)
finally:
    print("File Close")
```
**Explanation:**
- finally block always executes
- Whether exception occurs or not
- Guarantees resource cleanup (file close, DB close, etc.)
- This is the correct and safe approach
</details>
</details>

**Program: Handling IndexError Using try–except**
<details> <summary>Explanation</summary>

```python
a = [1, 3, 5]
try:
    print("first ", a[0])
    print("8th", a[8])
    print("second ", a[1])
except Exception as e:
    print(e)
    print("error")
```

**Execution**
`a = [1, 3, 5]`

- A list with 3 elements
- Valid indexes: 0, 1, 2<br>
`print("first ", a[0])`
- Accesses index 0<br>
` Output: 
first  1`
`print("8th", a[8])`
- Index 8 does not exist
- Raises IndexError
- Program control immediately jumps to the except block
- Remaining statement inside try<br>
`print("second ", a[1])`
- is skipped
<br>

`Exception Handling
except Exception as e:
    print(e)
    print("error")`


- e stores the error message
  <br>
  
` Output will be:
list index out of range
error
`

<br>

`Final Output
first  1
list index out of range
error
`

**Important Points to Remember**
- Once an exception occurs:
- Python stops executing the try block
- Jumps directly to the except
- Exception is a generic class that can catch all runtime errors
- This program demonstrates IndexError handling
           
</details>
</details>
  

#### Else Block 

<details> <summary>Show more</summary>
    
- The else block is used with the try–except statement.
- The try block contains the code that may cause an exception.
- The except block runs only if an exception occurs.
- The else block runs only if no exception occurs in the try block.

**Syntax**

```python
try:
    # Run this code
except:
    # Run this code if an exception occurs
else:
    # Run this code if no exception occurs
```

**Else Block in Exception Handling**
<details> <summary>Explanation</summary>
    
```python
def art(a, b):
    try:
        c = ((a + b) / (a - b))
    except ZeroDivisionError:
        print("a/b 0")
    else:
        print(c)

art(8.0, 9.0)
```
**Execution**
- Function call
`art(8.0, 9.0)`
- a = 8.0
- b = 9.0
- Try block calculation
  
` c = (a + b) / (a - b)`
- a + b = 8.0 + 9.0 = 17.0
- a - b = 8.0 - 9.0 = -1.0
- c = 17.0 / -1.0 = -17.0

**Exception check**
- Denominator is -1.0, not zero
- No ZeroDivisionError
- Else block executes
  
` print(c) `

**Output**
-17.0
</details>

**Else Block in Exception Handling2**
<details> <summary>Explanation</summary>

```python
def art(a, b):
    try:
        c = ((a + b) / (a - b))
    except ZeroDivisionError:
        print("a/b result is 0")
    else:
        print(c)

art(5.0, 5.0)
```

**Explanation**

- Function call
- a = 5.0
- b = 5.0
- Try block execution

`c = (a + b) / (a - b)`
- a + b = 10.0
- a - b = 0.0 
- Exception occurs
- Division by zero happens
- ZeroDivisionError is raised
- The except block executes

`print("a/b result is 0")`
- Else block
- Not executed because an exception occurred

`Output
a/b result is 0`
</details>

**Declaring Multiple Exceptions in Python**
<details> <summary>Explanation</summary>
- When a single try block may raise more than one type of exception, we can handle them together by declaring multiple exceptions in one except clause.
- Multiple exceptions are written inside parentheses, separated by commas.

**Syntax**
```python
try:
    # block of code
except (Exception1, Exception2, ..., ExceptionN):
    # block of code (runs if any listed exception occurs)
else:
    # block of code (runs if no exception occurs)
```
</details>

**Raising Exceptions in Python**
<details> <summary>Show more</summary>

- Python allows programmers to raise exceptions explicitly using the raise keyword.
- This is useful when you want to force an error based on a condition in your program.
- Syntax

` raise Exception_Class(value)`
- To access the exception value, the as keyword is used in the except block.
- Here, e is a reference variable that stores the exception message/value.

**Example**
```python
try:
    age = int(input("Enter your age: "))
    if age < 18:
        raise ValueError("Age must be 18 or above")
    print("Access granted")
except ValueError as e:
    print("Exception occurred:", e)
```

**Explanation**
- raise ValueError("Age must be 18 or above")
- Manually raises a ValueError exception.
- as e stores the exception message in variable e.
- The message can be accessed and printed using e.
  </details>

**Built-in Exceptions in Python**
<details> <summary>Show more</summary>

- Illegal operations in Python automatically raise exceptions.
- Python provides many built-in exception classes.
- These exceptions are raised when corresponding runtime errors occur.
-They help in error detection and handling.

**Common Built-in Exceptions**
| Exception Name      | Raised When                 |
| ------------------- | --------------------------- |
| `ZeroDivisionError` | Division by zero            |
| `ValueError`        | Invalid value passed        |
| `TypeError`         | Wrong data type used        |
| `IndexError`        | Index out of range          |
| `KeyError`          | Key not found in dictionary |
| `FileNotFoundError` | File does not exist         |
| `NameError`         | Variable not defined        |
| `AttributeError`    | Invalid attribute reference |

```
Syntax
locals()['__builtins__']
```

**Example**
`print(locals()['__builtins__'])`

**Explanation**

- locals() returns a dictionary of local symbol table.
- __builtins__ contains all built-in names.
- Built-in exceptions are available under this object.
</details>

**Python Built-in Exceptions**
<details> <summary>Show more</summary>
    
| **Exception**          | **Cause of Error**                                                    |
| ---------------------- | ----------------------------------------------------------------------|
| **AssertionError**     | Raised when an `assert` statement fails.                              |
| **AttributeError**     | Raised when an attribute reference or assignment fails.               |
| **EOFError**           | Raised when the `input()` function reaches the end-of-file condition. |
| **FloatingPointError** | Raised when a floating-point operation fails.                         |
| **GeneratorExit**       | Raised when a generator’s `close()` method is called.                               |
| **ImportError**         | Raised when an imported module cannot be found.                                     |
| **IndexError**          | Raised when the index of a sequence is out of range.                                |
| **KeyError**            | Raised when a key is not found in a dictionary.                                     |
| **KeyboardInterrupt**   | Raised when the user presses interrupt keys (`Ctrl + C` or `Delete`).               |
| **MemoryError**         | Raised when an operation runs out of memory.                                        |
| **NameError**           | Raised when a variable is not found in local or global scope.                       |
| **NotImplementedError** | Raised by abstract methods that are not implemented.                                |
| **OSError**             | Raised when a system-related operation causes an error.                             |
| **OverflowError**       | Raised when the result of an arithmetic operation is too large to be represented.   |
| **ReferenceError**      | Raised when a weak reference proxy accesses a garbage-collected object.             |
| **RuntimeError**        | Raised when an error does not fit any other exception category.                     |
| **StopIteration**       | Raised by the `next()` function when no further items are available in an iterator. |
</details>  

**Difference Between File Handling Functions in Python**
<details> <summary>Show more</summary>
    
| **Function**   | **Operation** | **What it Does**                                        | **Return Type**            | **Memory Usage**           | **Newline Handling**                   | **Typical Use Case**                         |
| -------------- | ------------- | ------------------------------------------------------- | -------------------------- | -------------------------- | -------------------------------------- | -------------------------------------------- |
| `read()`       | Read          | Reads the entire file or specified number of characters | `str`                      | **High** (for large files) | Preserves existing newlines (`\n`)     | Reading small files, full content processing |
| `readline()`   | Read          | Reads **one line at a time**                            | `str`                      | **Low**                    | Includes newline (`\n`) at end         | Log files, line-by-line processing           |
| `readlines()`  | Read          | Reads all lines and stores them in a list               | `list`                     | **High**                   | Each line includes `\n`                | When lines need indexing or list processing  |
| `write()`      | Write         | Writes a **single string** to a file                    | `int` (characters written) | **Low**                    | Does **not** add newline automatically | Writing single records                       |
| `writelines()` | Write         | Writes **multiple strings** (list/tuple) to a file      | `None`                     | **Low**                    | Does **not** add newline automatically | Writing multiple records                     |


</details>
</details>

try:
    a=1
    b=9
    print(a//b)
# Basic try–except Block 
try: 
    a=10
    b=0
    print(a//b)
except :
    print("Input Invalid")
# Using Exception Class
try: 
    a=int(input("enter the a : "))
    b=int(input("enter the b : "))
    print(a//b)
except Exception:
    print("Input Invalid")
#Using Exception as e
try: 
    a=int(input("enter the a : "))
    b=int(input("enter the b : "))
    print(a//b)
except Exception as e:
    print(e)
# Program: try with except (No finally)
try: 
    print("File Open")
    a=int(input("enter the a : "))
    b=int(input("enter the b : "))
    print(a//b)
    print("File Close")
except Exception as e:
    print(e)
# Program: try–except with manual file closing
try: 
    print("File Open")
    a=int(input("enter the a : "))
    b=int(input("enter the b : "))
    print(a//b)
    print("File Close")
except Exception as e:
    print(e)
    print("File Close")
# Program: try–except–finally
try: 
    print("File Open")
    a=int(input("enter the a : "))
    b=int(input("enter the b : "))
    print(a//b)
    print("File Close")
except Exception as e:
    print(e)
finally:
    print("File Close")
# Program: try–except–finally
a=[1,3,5]
try:
    print("first ", a[0])
    print("8th", a[8])
    print("second ", a[1])
    
except Exception as e:
    print(e)
    print("error")

# Else Block in Exception Handling
def art(a,b):
    try:
        c=((a+b)/(a-b))
    except ZeroDivisionError:
        print("a/b 0")
    else:
        print(c)
art(8.0,9.0)

    
# Else Block in Exception Handling2
def art(a,b):
    try:
        c=((a+b)/(a-b))
    except ZeroDivisionError:
        print("a/b result is 0")
    else:
        print(c)
art(5.0,5.0)
# Raising Exceptions in Python
try:
    age = int(input("Enter your age: "))
    if age < 18:
        raise ValueError("Age must be 18 or above")
    print("Access granted")
except ValueError as e:
    print("Exception occurred:", e)
## Automated Log File Health Monitoring System
<details>
<summary>Problem Statement</summary>
    


- A company maintains server activity logs stored as text files. Each line in the log file represents a system event, which may contain the keywords INFO, WARNING, or ERROR. The system analyzes the uploaded log file and determines the overall health of the server based on the frequency of error events. 
 
The health evaluation rules are as follows: 

- If the number of ERROR entries is greater than 10, the system status is "CRITICAL" 
- If the number of ERROR entries is between 5 and 10, the system status is "WARNING" 
- If the number of ERROR entries is less than 5, the system status is "NORMAL" 
- If the log file contains no records, the system status is "NO ACTIVITY" 
- If the log file is missing, unreadable, or corrupted, the output must be "INVALID LOG FILE" 
The system must allow users to upload the log file via a Gradio interface and display the analysis 
result. 
</details>

#Automated Log File Health Monitoring System
import gradio as gr

def an_health(file):
    try:
        with open(file.name, "r") as fI:
            liS = fI.readlines()

        if len(liS) == 0:
            return "System Status: NO ACTIVITY"

        errorcount = 0
        for LI in liS:
            if "ERROR" in LI:
                errorcount += 1

        if errorcount > 10:
            status = "CRITICAL"
        elif 5 <= errorcount <= 10:
            status = "WARNING"
        else:
            status = "NORMAL"

        return f"Total Errors: {errorcount}\nSystem Status: {status}"

    except:
        return "INVALID HEALTH LOG .TXT FILE"


gr.Interface(
    fn=an_health,
    inputs=gr.File(label="Plz Upload Health Log File (.txt)"),
    outputs="text",
    title="Log File Health Monitoring System"
).launch()
## Smart Resume Eligibility Analyzer

<details>
<summary> Problem Statement </summary>
    


- An online recruitment platform receives resumes uploaded by candidates in the form of text files. Each resume contains a list of technical skills separated by commas.Due to different user behaviors, resumes may be empty, incomplete, or uploaded in an incorrect format. 
 
The system reads the uploaded resume file and determines the candidate’s eligibility based on the 
number of skills present. 
The eligibility rules are defined as follows: 
- If the resume contains zero skills, the candidate status is "REJECTED" 
- If the resume contains 1 to 2 skills, the status is "NOT ELIGIBLE" 
- If the resume contains 3 to 6 skills, the status is "ELIGIBLE" 
- If the resume contains more than 6 skills, the status is "HIGHLY ELIGIBLE" 
- If the resume file is empty, unreadable, or corrupted, the output must be "INVALID 
RESUME FILE" 
- If the uploaded file format is not .txt, the output must be "INVALID INPUT FORMAT" 
 
The system must be implemented using Python File Handling, Exception Handling, and a Gradio
based user interface that allows users to upload the resume file and view the eligibility result.

</details>
# Smart Resume Eligibility Analyze
import gradio as gr

def analyze_resume(file):
    try:
        # Check file format
        if not file.name.endswith(".txt"):
            return "INVALID INPUT .TXT FORMAT"

        # Read file
        with open(file.name, "r") as f:
            content = f.read().strip()

        # Check empty file
        if content == "":
            return "INVALID RESUME .TXT FILE"

        # Split skills by comma
        skills = [s.strip() for s in content.split(",") if s.strip()]
        skill_count = len(skills)

        # Eligibility rules
        if skill_count == 0:
            status = "REJECTED"
        elif skill_count <= 2:
            status = "NOT ELIGIBLE"
        elif skill_count <= 6:
            status = "ELIGIBLE"
        else:
            status = "HIGHLY ELIGIBLE"

        return f"Skill Count: {skill_count}\nCandidate Status: {status}"

    except:
        return "INVALID RESUME .TXT FILE"

#gradio interface
gr.Interface(
    fn=analyze_resume,
    inputs=gr.File(label="PLZ Upload Resume (.txt)"),
    outputs="text",
    title="Smart Resume Eligibility Analyzer"
).launch()

##  Student Examination Eligibility Evaluation System 
<details> <summary> Problem Statement </summary>


- A university stores student attendance records in a text file. Each record contains a student roll number and attendance percentage separated by a comma. Because attendance data is entered manually, the file may contain invalid or non-numeric entries. 
 
The system reads the attendance file and determines each student’s eligibility for the examination based on the following rules: 
- If attendance is 85% or above, the student is "ELIGIBLE FOR EXAM" 
- If attendance is between 65% and 84%, the student status is "CONDONATION REQUIRED" 
- If attendance is below 65%, the student is "NOT ELIGIBLE" 
- Records with invalid or missing attendance values must be ignored 
- If the file is empty, missing, or unreadable, the output must be "INVALID INPUT FILE" 
 
The system must be developed using Python file operations, exception handling, and a Gradio
based user interface to upload the attendance file and display the eligibility report. 
 
</details>

# Student Examination Eligibility Evaluation System
import gradio as gr

def evaluate_attendance(file):
    try:
        # open and read file
        with open(file.name, "r") as f:
            lines = f.readlines()

        if len(lines) == 0:
            return "INVALID INPUT .TXT FILE"

        result = ""

        for line in lines:
            try:
                roll, attendance = line.strip().split(",")
                attendance = float(attendance)

                if attendance >= 85:
                    status = "ELIGIBLE FOR EXAM"
                elif attendance >= 65:
                    status = "CONDONATION REQUIRED"
                else:
                    status = "NOT ELIGIBLE"

                result += f"Roll No: {roll.strip()} - {status}\n"

            except:
                # Ignore invalid records
                continue

        return result.strip()

    except:
        return "INVALID INPUT .TXT FILE"


gr.Interface(
    fn=evaluate_attendance,
    inputs=gr.File(label="PLZ Upload Attendance File (.txt)"),
    outputs="text",
    title="Student Examination Eligibility System"
).launch()
<h2>Gradio</h2>
<details>
<summary>Show more</summary>
<h5> What is Gradio? </h5>
Gradio is an open-source Python library that helps you create interactive user interfaces for your machine learning models or Python functions - with just a few lines of code!

<h5> It allows </h5>

- Rapid prototyping
- Sharing apps easily with others via links
- No need for web development knowledge!

<h5>Use Cases:</h5>

- Machine Learning Demos
- Image, Text, or Audio Tools
- Fun Python Apps (like Emoji Translators!)

</details>

<h2> Module, Package, and Library </h2>
<details><summary>show more</summary>
<h5>What is a Module?</h5>
A module is a single Python file (.py) that contains:

- Functions
- Classes
- Variables

<h5>What is a Package?</h5>
A package is a folder (directory) that contains multiple modules.
It usually contains a special file called __init__.py.

Example Structure:

calculator/
│
├── __init__.py
├── add.py
├── sub.py


<h5>What is a Library?</h5>
A library is a collection of packages and modules designed to provide specific functionality.
It is bigger than a package.
Examples of Python Libraries:

NumPy – Used for numerical calculations
```
import numpy as np
arr = np.array([1, 2, 3])
```

Pandas – Used for data analysis
```
import pandas as pd
```

Matplotlib – Used for plotting graphs
TensorFlow – Used for Machine Learning


| Feature | Module            | Package           | Library                |
| ------- | ----------------- | ----------------- | ---------------------- |
| Meaning | Single `.py` file | Folder of modules | Collection of packages |
| Size    | Small             | Medium            | Large                  |
| Example | `mymath.py`       | `calculator/`     | NumPy, Pandas          |


</details>


import pandas as pd
file=pd.read


import pandas as pd
data={
    "Name":["Alice","Bob","Charlie"],
    "Marks":[85,93,90]
}
df=pd.DataFrame(data)
print(df)
import math
result=math.sqrt(25)
print("square Root:",result)

import math
r = float(input("Enter radius: "))
area = math.pi * r**2
print("Area of Circle =", area)


!pip list

!pip list --format=freeze

help('module')
## Automation
<details><summary>show mory</summary>
Automation is the use of software systems to perform repetitive tasks automatically without continuous human intervention.
       <b> or</b><br>
Automation means the computer does the work for us automatically.

<br>


<b>Basic Flow of Automation : </b><br>
<b> Input → Processing (Logic) → Action (Output)</b>

 Input : User gives data or instruction to the system.<br>
 Processing (Logic) : The system applies predefined rules and conditions.<br>
 Output (Action) : The system performs the task and gives result automatically.<br>

- Automation reduces manual effort, human error, and time consumption.
- It works based on predefined rules, conditions, and programmed instructions.
- Automation systems are designed to be scalable, consistent, and efficient in real-world environments



#### AUTOMATION UNLOCKED

- REPETITIVE TASK EXECUTION
Software performs identical tasks repeatedly without human input.
<b> EXAMPLE:</b>
Send 100 daily attendance alerts automatically.

- RULE-BASED DECISION MAKING
Predefined if/else logic processes inputs deterministically.
<b>EXAMPLE:</b>
If attendance < 60% send email, else → log OK.

- INPUT → LOGIC → ACTION FORMULA
 Structured data flow: Data In → Process → Result Out.
<b>EXAMPLE:</b>
CSV attendance → filter logic → email alerts.

- MINIMAL HUMAN INTERVENTION
Runs independently after initial setup (cron/scheduler).
<b>EXAMPLE:</b>
Daily 9AM execution, no manual start required.

- MEASURABLE BUSINESS OUTCOME
Quantifiable ROI through time, cost, and error reduction.
<b>EXAMPLE:</b>
625 manual hours → 25 automated hours = 96% savings.

#### Types of Automation

**1. Robotic Process Automation (RPA)** : Software bots automate repetitive computer tasks.

**2. Cognitive Automation** : Uses AI to make smart decisions.

**3. Industrial Automation** : Machines automate factory work.

**4. Business Process Automation (BPA)** : Automates business workflows like payroll and billing.

**5. Home Automation** : Controls home devices automatically.

**6. Autonomous Systems** : Systems that work independently without human control.

#### 5 Key Automation Types

| Type                              | Description                     | Python Tools        |
| --------------------------------- | ------------------------------- | ------------------- |
| Robotic Process Automation (RPA)  | GUI automation (clicks, typing) | PyAutoGUI, Selenium |
| Business Process Automation (BPA) | Workflow orchestration          | Airflow             |
| Industrial Automation             | Manufacturing / robots          | PyModbus, ROS       |
| Home Automation                   | Smart devices / IoT             | Home Assistant      |
| Cognitive Automation              | AI/ML decision making           | LangChain, OpenAI   |

##### Additional Example

| Type                | Description                                            | Tools                               |
| ------------------- | ------------------------------------------------------ | ----------------------------------- |
| Business Automation | Payroll systems, CRM automation, Email marketing tools | CRM Software, Email Marketing Tools |



#### Why Automate ? 
- Improves productivity
- Reduces human error
- Enhances reliability
- Ensures system availability
- Enables scalability

#### Trends in Automation 
- Artificial Intelligence
- Robotics
- Internet of Things (IoT)
- Cloud Computing
- Augmented Reality

<details>
<summary>GUI Automation Using Python</summary>


#### What is PyAutoGUI?
PyAutoGUI is a cross-platform Python library for GUI automation.

##### Purpose

It allows you to programmatically control the mouse, keyboard, and screen to automate repetitive tasks.

##### Platforms

Works on Windows, macOS, and Linux.


##### Use Cases

Automating workflows, testing applications, creating bots, taking screenshots, and simulating user interactions.


#### Applications of Automation

##### Automation of Repetitive Tasks

Save time by automating typing, clicking, and navigation.

##### Software Testing

Simulate user input for GUI testing.

##### Productivity Boost

Automate routine actions like filling forms or saving files.

##### Creative Uses

Drawing shapes in Paint, creating bots for games, or generating automated reports.


##### Learning Tool

Helps beginners understand event-driven programming and automation concepts.


#### Key Features of PyAutoGUI

| Feature           | Description                    | Example                                  |
| ----------------- | ------------------------------ | ---------------------------------------- |
| Mouse Control     | Move, click, drag, scroll      | `pyautogui.click(x, y)`                  |
| Keyboard Control  | Type text, press keys, hotkeys | `pyautogui.typewrite("Hello")`           |
| Screenshot        | Capture screen images          | `pyautogui.screenshot("img.png")`        |
| Image Recognition | Locate elements on screen      | `pyautogui.locateOnScreen("button.png")` |
| Fail-Safe         | Move mouse to top-left to stop | Built-in safety mechanism                |


`pyautogui` -> gives access to mouse, keyboard, and screen automation.
</details>
<details>
<summary>RPA</summary>

#### What is RPA?


RPA excels at repetitive, rule-based tasks with structured data, like following a strict recipe.

RPA is software automation that mimics human actions in digital systems — like clicking, typing, copying, and pasting.

##### Core Foundation

Rule-based logic (not true AI).
It follows predefined workflows.


##### RPA Tasks

* Extracting data from documents
* Filling forms
* Moving files between systems
* Sending routine notifications


##### Strengths of RPA

* Reliable and consistent outcomes
* Fast execution
* Reduces human error
* Frees employees for higher-value work
</details>

#### Automation vs AI Workflow vs AI Agent

| Aspect          | Automation                                          | AI Workflow                                                       | AI Agent                                          |
| --------------- | --------------------------------------------------- | ----------------------------------------------------------------- | ------------------------------------------------- |
| Definition      | Executes predefined, rule-based tasks automatically | Calls an LLM (Large Language Model) via API for one or more steps | Performs non-deterministic tasks autonomously     |
| Core Foundation | Boolean logic                                       | Boolean logic + Fuzzy logic                                       | Autonomous reasoning                              |
| Strengths       | Deterministic, fixed tasks                          | Deterministic tasks with flexibility                              | Adaptive, non-deterministic tasks                 |
| Capabilities    | Reliable outcomes, fast execution                   | Handles complex rules, good at pattern recognition                | Highly adaptive, simulates human-like reasoning   |
| Weaknesses      | Limited to programmed tasks, cannot adapt           | Needs training data, harder to debug                              | Less predictable, slower execution                |
| Example         | Send a Slack notification when a new lead signs up  | Analyze and route leads using ChatGPT                             | Perform full internet search and update lead info |



##### Decoding: Automation vs AI Workflows vs AI Agents

* **Automation** → Fixed rules, predictable results
* **AI Workflow** → Uses AI for decision steps
* **AI Agent** → Acts independently and adapts dynamically



    
</details>





! pip install emoji

import gradio as gr
import emoji

def emoji_to_name(user_input):
    return emoji.demojize(user_input)

demo = gr.Interface(
    fn=emoji_to_name,
    inputs=gr.Textbox(label="Enter Emoji 😊"),
    outputs=gr.Textbox(label="Emoji Name"),
    title="😊 Emoji to Name Translator"
)

demo.launch()





pip install pyautogui





import pyautogui
import time
import os

# Open notepadHell
os.system("notepad")

# Wait 2 seconds
time.sleep(2)

# Type text
pyautogui.typewrite("Hello!, this is auto typing program!", interval=0.1)

pyautogui.press("enter")

pyautogui.typewrite("Python is writing this automatically.", interval=0.1)

# Save file
pyautogui.hotkey("ctrl", "s")

time.sleep(1)

pyautogui.typewrite("pyautogui_note2.txt", interval=0.1)

pyautogui.press("enter")
PythoHen is writing this automatically.pyautogui_note.txt
Hello!, this is auto typing program!
PythoHen is writing this automatically.pyautogui_note.txt

import os




    os.remove(pyautogui_note.txt)
    print("File deleted")
else:
    print("File not found")
import pyautogui
import time
import os

# Open notepadHell
os.system("notepad")

# Wait 2 seconds
time.sleep(2)

# Type text
pyautogui.typewrite("Hello!, this is auto typing program!", interval=0.1)

pyautogui.press("enter")

pyautogui.typewrite("Python is writing this automatically.", interval=0.1)

# Save file
pyautogui.hotkey("ctrl", "s")

time.sleep(1)

pyautogui.typewrite("pyautogui_note2.txt", interval=0.1)

pyautogui.press("enter")

#screenshot taken
import pyautogui
import time
import os

time.sleep(2)
screenshot=pyautogui.screenshot()
screenshot.save("abc.jpg")


import pyautogui
import time

time.sleep(1)

# Take screenshot
screenshot = pyautogui.screenshot()

# Save screenshot
screenshot.save("my_screenshot.png")


import pyautogui
import time
import os

os.system("notepad")

time.sleep(2)

# Type text
pyautogui.typewrite("Hello Nana, this is auto typing program!", interval=0.1)
pyautogui.press("enter")
pyautogui.typewrite("Python is writing this automatically.", interval=0.1)

# Save file
pyautogui.hotkey("ctrl", "s")
time.sleep(1)
pyautogui.typewrite("pyautogui_note.txt", interval=0.1)
pyautogui.press("enter")

# Wait before screenshot
time.sleep(2)

# Take Screenshot
screenshot = pyautogui.screenshot()
screenshot.save("notepad_screenshot.png")

print("Typing and Screenshot completed successfully!")
Python is writing this automatically.pyautogui_note.txt




import pyatogui
import time

for i in range
import pyautogui
import time
 
for i in range(3):  # Take 3 screenshots
    scre. Sleep(5)enshot = pyautogui.screenshot()
    filename = f"screenshot_{int(time.time())}.png"
    screenshot.save(filename)
    print(f"Saved {filename}")
    time
import pyautogui
import time
import pyautogui
import time
import os
  example)
os.system("mspaint")
# Open Paint (Windows
time.sleep(3)
 
# Move mouse to canvas area.
pyautogui.moveTo(400, 400, duration=1)
 
# Draw a square
for _ in range(4):
    pyautogui.dragRel(100, 0, duration=1)  # Right
    pyautogui.dragRel(0, 100, duration=1)  # Down
    pyautogui.dragRel(-100, 0, duration=1) # Left
    pyautogui.dragRel(0, -100, duration=1) # Up
pyautogui.


### Top 5 AI Tools To build Agentic AI System

1. LangChain
2. CrewAI
3. AutoGen
4. AutoGpt
5. LlamaIndex

##### 1. LangChain 

**What is it?**
LangChain is a framework used to build intelligent applications using Large Language Models (LLMs), and it can be easily implemented and tested in **Jupyter Notebook** to develop AI agents with tools, memory, and custom logic.

**Core Features:**

* **Chains:** Sequences of LLM and logic steps executed in notebook cells.
* **Agents:** LLMs that decide actions and use tools directly from the notebook environment.
* **Memory:** Stores conversation context during notebook execution.
* **Tools:** Connect to APIs, databases, or Python functions inside the notebook.
* **Retrieval Augmented Generation (RAG):** Retrieve documents and generate accurate responses.

**Real-Time Applications:**

* Q&A bots for college materials
* AI tutor bots for assignments
* Academic search assistants
* SQL query generation bots


##### 2. AutoGen

**What is it?**
AutoGen is a framework developed by Microsoft that enables **multi-agent collaboration using LLMs**, where multiple AI agents work together like a team to solve complex tasks.

**Core Features**

* **Role-based Agents:** Agents like *Assistant* and *UserProxy* perform different roles.
* **Multi-Agent Group Chat:** Agents communicate with each other to complete tasks.
* **Tools & Function Execution:** Agents can run code, APIs, and external tools.
* **Human-in-the-Loop:** Humans can monitor or guide the agents during execution.

**Real-Time Applications**

* Research assistants (writer + editor agents)
* Software engineering automation bots
* Content generator teams
* Simulated student–teacher bots for learning systems



##### 3. Flowise

**What is it?**
Flowise is a **no-code visual builder based on LangChain** that allows users to create powerful AI workflows using a drag-and-drop interface without writing code.

**Core Features**

* **Drag-and-Drop Visual Editor** to design AI workflows
* Supports LLMs such as OpenAI, Ollama, and Cohere
* Integrates with vector databases like Pinecone and ChromaDB
* Can be deployed **locally or in the cloud**

**Real-Time Applications**

* Chat with notes, PDFs, and websites
* Academic bots for resume review
* Internal knowledge assistants for colleges
* Grievance redressal chatbots

##### 4. SuperAGI

**What is it?**

* SuperAGI is an **autonomous agent framework** that builds agents which can **think, plan, and act independently.** *(Note: "think, plan, and act" are underlined in red in the image).*

**Core Features:**

* Set goals, and agents autonomously act
* Visual dashboards to track agent progress
* Large library of built-in tools
* **Git-based workflows** *(Note: This item is circled in red in the image).*


**Real-Time Applications:**

* Autonomous academic research bots
* Student email bots
* Fee payment follow-up agents
* Assignment plagiarism checkers

##### 5. CrewAI

**What is it?**
CrewAI is an **open-source multi-agent orchestration framework** where specialized AI agents collaborate like a **project team** to complete complex, multi-step tasks using defined roles, goals, and workflows.


**Core Features**

**1️ Role-Based Agents**
Agents can be customized with **specific roles, goals, backstories, and tools** to perform specialized tasks.

**2️ Managed Collaboration**
Supports **sequential or hierarchical workflows**, where agents complete tasks step-by-step or under a manager agent.

**3️ Tool Integration**
Agents can connect to **APIs, search engines, databases, and custom tools** to perform real-world operations.

**4️ Flexible LLM Support**
Works with different language models such as **OpenAI**, **Claude**, and local models.

**5️ Transparent Execution**
Agents communicate with each other, **share context, and pass outputs** to complete the overall task.



**Real-Time Applications**

* Research teams (researcher + writer + editor agents)
* Automated content creation systems
* Business workflow automation
* Software development assistant teams
