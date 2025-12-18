<h1>Python Fundamentals – Detailed Explanation</h1>
<hr>

<h2>Python Variables</h2>
<p>
A variable in Python is a named location in memory that stores data.
When we assign a value to a variable, Python automatically decides the
type of data stored. This is called <b>dynamic typing</b>.
</p>

<p>
Variables make programs flexible and reusable. Instead of using fixed
values repeatedly, we store values in variables and use them whenever required.
</p>

<h3>Important Rules for Variables</h3>
<ul>
  <li>Variable names must start with a letter or underscore (_)</li>
  <li>They cannot start with a number</li>
  <li>Only letters, numbers, and underscores are allowed</li>
  <li>Python is case-sensitive (age and Age are different)</li>
  <li>Keywords like if, for, while cannot be used as variable names</li>
</ul>

<h3>Examples</h3>
<pre>
x = 10        # integer variable
name = "Ram" # string variable
_marks = 90
</pre>

<p>
In the above example, Python automatically assigns data types to variables
based on the values stored.
</p>

<hr>

<h2>Python Data Types</h2>
<p>
Data types specify what kind of data a variable can store.
Python provides built-in data types to handle numbers, text, and collections.
</p>

<h3>Numeric Data Types</h3>
<p>
Numeric data types are used to store numerical values.
</p>

<ul>
  <li><b>int</b> – stores whole numbers (positive or negative)</li>
  <li><b>float</b> – stores decimal values</li>
  <li><b>complex</b> – stores real and imaginary values</li>
</ul>

<pre>
a = 25
b = 10.5
c = 3 + 4j

print(type(a))
print(type(b))
print(type(c))
</pre>

<p>
Integers are used for counting, floats for precision values, and complex
numbers mainly in scientific calculations.
</p>

<hr>

<h3>String Data Type</h3>
<p>
A string is a sequence of characters enclosed in single, double,
or triple quotes. Strings are <b>immutable</b>, meaning once created,
they cannot be changed.
</p>

<pre>
text = "Python Programming"
print(text[0])      # First character
print(text[-1])     # Last character
print(text[0:6])    # Slicing
</pre>

<h3>Important String Operations</h3>
<pre>
s = " python language "
print(s.upper())
print(s.lower())
print(s.strip())
print(s.replace("python", "java"))
print(s.split())
</pre>

<p>
Strings are widely used for handling user input, messages, and text processing.
</p>

<hr>

<h3>List Data Type</h3>
<p>
A list is an ordered, mutable collection of elements.
It allows duplicate values and different data types in a single list.
</p>

<pre>
data = [10, "Python", 3.5]
data.append(100)
data[0] = 50
print(data)
</pre>

<p>
Lists are commonly used when data needs to be modified frequently.
</p>

<hr>

<h3>Tuple Data Type</h3>
<p>
A tuple is similar to a list, but it is immutable.
Once created, elements cannot be added, removed, or modified.
</p>

<pre>
t = (10, 20, 30)
print(t[1])
</pre>

<p>
Tuples are used to protect data from accidental modification.
</p>

<hr>

<h3>Set Data Type</h3>
<p>
A set is an unordered collection of unique elements.
Duplicate values are automatically removed.
</p>

<pre>
s = {1, 2, 3, 3, 4}
print(s)
</pre>

<h3>Set Operations</h3>
<pre>
a = {1, 2, 3}
b = {3, 4, 5}
print(a.union(b))
print(a.intersection(b))
</pre>

<p>
Sets are mainly used for mathematical operations and removing duplicates.
</p>

<hr>

<h3>Dictionary Data Type</h3>
<p>
A dictionary stores data in key-value pairs.
Keys must be unique and immutable, while values can be any data type.
</p>

<pre>
student = {
  "name": "Ravi",
  "age": 21,
  "course": "Python"
}

print(student["name"])
print(student.get("age"))
</pre>

<p>
Dictionaries are used to represent structured data like records.
</p>

<hr>

<h2>Type Conversion</h2>
<p>
Type conversion is the process of converting one data type into another.
It can be implicit or explicit.
</p>

<h3>Implicit Type Conversion</h3>
<pre>
x = 10
y = 5.5
z = x + y
print(z)
print(type(z))
</pre>

<p>
Python automatically converts int to float to avoid data loss.
</p>

<h3>Explicit Type Conversion</h3>
<pre>
a = "100"
b = int(a)
print(b + 20)
</pre>

<p>
Explicit conversion is done manually using functions like int(), float(), str().
</p>

<hr>

<h2>Python Operators</h2>

<h3>Arithmetic Operators</h3>
<p>
Used to perform mathematical operations.
</p>

<pre>
a = 10
b = 3
print(a + b)
print(a - b)
print(a * b)
print(a / b)
print(a % b)
</pre>

<h3>Comparison Operators</h3>
<p>
Used to compare values and return True or False.
</p>

<pre>
print(10 > 5)
print(10 == 5)
print(10 != 5)
</pre>

<h3>Logical Operators</h3>
<p>
Used to combine conditions.
</p>

<pre>
x = True
y = False
print(x and y)
print(x or y)
print(not x)
</pre>

<h3>Membership Operators</h3>
<pre>
nums = [1, 2, 3]
print(2 in nums)
print(5 not in nums)
</pre>

<h3>Identity Operators</h3>
<pre>
a = 10
b = 10
print(a is b)
print(a is not b)
</pre>

<hr>

<h2>Loops</h2>
<p>
Loops are used to execute a block of code repeatedly.
</p>

<h3>for Loop</h3>
<p>
Used to iterate over sequences like lists, strings, and ranges.
</p>

<pre>
for i in range(1, 6):
    print(i)
</pre>

<h3>while Loop</h3>
<p>
Executes as long as the condition is true.
</p>

<pre>
i = 1
while i <= 5:
    print(i)
    i += 1
</pre>

<h3>Loop Control Statements</h3>
<pre>
for i in range(1, 6):
    if i == 3:
        continue
    if i == 5:
        break
    print(i)
</pre>

<hr>

<h2>Functions</h2>
<p>
A function is a reusable block of code that performs a specific task.
Functions improve code readability and reduce repetition.
</p>

<h3>Function Definition</h3>
<pre>
def greet():
    print("Hello Python")

greet()
</pre>

<h3>Function with Parameters and Return</h3>
<pre>
def add(a, b):
    return a + b

print(add(10, 20))
</pre>

<h3>Default Arguments</h3>
<pre>
def welcome(name="User"):
    print("Welcome", name)

welcome()
welcome("Python")
</pre>

<hr>

<h2>Lambda Functions</h2>
<p>
Lambda functions are anonymous functions written in a single line.
They are mainly used for short operations.
</p>

<pre>
square = lambda x: x * x
print(square(5))
</pre>

<hr>

<h2>File Handling</h2>
<p>
File handling allows programs to read data from files and write data into files.
</p>

<pre>
file = open("data.txt", "w")
file.write("Hello Python")
file.close()

file = open("data.txt", "r")
print(file.read())
file.close()
</pre>

<hr>

<h2>Final Conclusion</h2>
<p>
This document explains Python fundamentals in detail, covering variables,
data types, operators, loops, functions, lambda expressions, and file handling
with clear examples. These concepts are essential for examinations,
real-world programming, and advanced Python learning.
</p>
