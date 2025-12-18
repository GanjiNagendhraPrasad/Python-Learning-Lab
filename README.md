<hr>

<h2>8. Control Flow Statements (Decision Making)</h2>
<p>
Control flow statements allow a program to make decisions and execute different blocks of code
based on conditions. These statements are essential for building logic in real-world applications.
</p>

<h3>8.1 if Statement</h3>
<p>
The <b>if</b> statement executes a block of code only when the given condition is true.
Conditions usually use comparison or logical operators.
</p>

<pre>
age = 20
if age >= 18:
    print("Eligible to vote")
</pre>

<p><b>Explanation:</b>  
If the condition <code>age >= 18</code> is true, the message is printed. Otherwise, nothing happens.</p>

<h3>8.2 if–else Statement</h3>
<p>
The <b>if–else</b> statement provides two execution paths: one when the condition is true and
another when it is false.
</p>

<pre>
age = 16
if age >= 18:
    print("Eligible to vote")
else:
    print("Not eligible")
</pre>

<h3>8.3 if–elif–else Statement</h3>
<p>
Used when multiple conditions must be checked sequentially. Python evaluates conditions
from top to bottom.
</p>

<pre>
marks = 75
if marks >= 90:
    print("Grade A")
elif marks >= 60:
    print("Grade B")
else:
    print("Grade C")
</pre>

<h3>8.4 Nested if Statements</h3>
<p>
A nested if means placing an if statement inside another if statement.
This is useful for checking multiple related conditions.
</p>

<pre>
age = 20
citizen = True

if age >= 18:
    if citizen:
        print("Eligible to vote")
    else:
        print("Citizenship required")
</pre>

<p><b>Usage:</b>  
Used in validations, decision-making systems, authentication logic, and rule-based programs.</p>

<hr>

<h2>9. Control Flow Practice (Problem Solving)</h2>
<p>
This section focuses on applying control flow concepts to solve logical and real-time problems.
Practicing these problems improves analytical thinking and confidence in writing conditions.
</p>

<h3>Example: Check Even or Odd</h3>
<pre>
num = 7
if num % 2 == 0:
    print("Even number")
else:
    print("Odd number")
</pre>

<h3>Example: Largest of Two Numbers</h3>
<pre>
a = 10
b = 20
if a > b:
    print("a is larger")
else:
    print("b is larger")
</pre>

<p><b>Usage:</b>  
Helps in interviews, competitive programming, and real-world logic building.</p>

<hr>

<h2>10. Functions – In Detail</h2>
<p>
Functions are reusable blocks of code that perform a specific task.
They reduce repetition, improve readability, and make programs easier to maintain.
</p>

<h3>10.1 Why Use Functions?</h3>
<ul>
  <li>Avoid code repetition</li>
  <li>Improve program structure</li>
  <li>Easy debugging and maintenance</li>
</ul>

<h3>10.2 Function Without Parameters</h3>
<pre>
def greet():
    print("Welcome to Python")

greet()
</pre>

<p>
This function performs a fixed task every time it is called.
</p>

<h3>10.3 Function With Parameters</h3>
<pre>
def add(a, b):
    return a + b

result = add(10, 20)
print(result)
</pre>

<p>
Parameters allow passing data into a function, making it more flexible.
</p>

<h3>10.4 Return Statement</h3>
<p>
The <b>return</b> statement sends a value back to the caller so it can be reused.
</p>

<pre>
def square(n):
    return n * n

print(square(5))
</pre>

<h3>10.5 Default Arguments</h3>
<pre>
def welcome(name="User"):
    print("Welcome", name)

welcome()
welcome("Python")
</pre>

<p><b>Usage:</b>  
Functions are used in automation, data processing, applications, and large-scale projects.</p>

<hr>

<h2>11. Lambda (Anonymous) Functions</h2>
<p>
Lambda functions are small, one-line anonymous functions.
They are used when a simple operation is needed for a short time.
</p>

<h3>Syntax</h3>
<pre>
lambda arguments : expression
</pre>

<h3>Example</h3>
<pre>
square = lambda x: x * x
print(square(5))
</pre>

<p>
Lambda functions are commonly used with built-in functions like <b>map()</b>, <b>filter()</b>,
and <b>reduce()</b>.
</p>

<h3>Example with filter()</h3>
<pre>
nums = [1, 2, 3, 4, 5]
even_nums = list(filter(lambda x: x % 2 == 0, nums))
print(even_nums)
</pre>

<p><b>Usage:</b>  
Used in data transformations, functional programming, and clean code practices.</p>

<hr>

<h2>12. File Handling in Python</h2>
<p>
File handling allows Python programs to read data from files and write data to files.
This is important for data storage, logging, and report generation.
</p>

<h3>12.1 Opening a File</h3>
<pre>
file = open("data.txt", "w")
file.write("Hello Python")
file.close()
</pre>

<h3>12.2 File Modes</h3>
<ul>
  <li><b>r</b> – Read</li>
  <li><b>w</b> – Write (overwrites file)</li>
  <li><b>a</b> – Append</li>
</ul>

<h3>12.3 Reading a File</h3>
<pre>
file = open("data.txt", "r")
content = file.read()
print(content)
file.close()
</pre>

<h3>12.4 Using with Statement</h3>
<p>
Automatically closes the file after execution.
</p>

<pre>
with open("data.txt", "r") as file:
    print(file.read())
</pre>

<p><b>Usage:</b>  
Used in data storage, file processing, logs, and real-world applications.</p>

<hr>

<h2>Final Conclusion</h2>
<p>
This repository provides a complete and detailed understanding of Python fundamentals,
including variables, data types, operators, control flow statements, loops, functions,
lambda expressions, and file handling.
By practicing these concepts, learners build strong logical skills and a solid foundation
for advanced Python programming and real-world projects.
</p>
