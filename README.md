<h1>Python Fundamentals</h1>
<hr>

<h2>Python Variables</h2>
<p>
Variables are used to store data values in memory. In Python, a variable is created
the moment a value is assigned to it. Python is a dynamically typed language, so you
do not need to specify the data type explicitly.
</p>

<p>
Variables help make programs readable, reusable, and flexible.
</p>

<h3>Rules for Variable Names</h3>
<ul>
  <li>Must start with a letter or underscore (_)</li>
  <li>Cannot start with a number</li>
  <li>Can contain letters, numbers, and underscores</li>
  <li>Case-sensitive</li>
  <li>Cannot be Python keywords</li>
</ul>

<pre>
age = 20
name = "Python"
_totalMarks = 450
</pre>

<hr>

<h2>Python Data Types</h2>
<p>
Data types define the type of data stored in a variable. Python provides several
built-in data types to handle different kinds of values.
</p>

<h3>Numeric Data Types</h3>
<p>
Numeric data types are used to store numerical values.
</p>

<ul>
  <li><b>int</b> – whole numbers</li>
  <li><b>float</b> – decimal numbers</li>
  <li><b>complex</b> – numbers with real and imaginary parts</li>
</ul>

<pre>
a = 10
b = 3.14
c = 4 + 5j
print(type(a))
print(type(b))
print(type(c))
</pre>

<hr>

<h3>String Data Type</h3>
<p>
A string is a sequence of characters enclosed in single quotes, double quotes,
or triple quotes. Strings are immutable, meaning they cannot be changed after creation.
</p>

<pre>
text = "Hello Python"
print(text[0])
print(text[-1])
print(text[0:5])
</pre>

<h4>String Methods</h4>
<pre>
s = " python programming "
print(s.upper())
print(s.lower())
print(s.strip())
print(s.replace("python", "java"))
print(s.split())
</pre>

<hr>

<h3>List Data Type</h3>
<p>
A list is an ordered and mutable collection of elements. Lists allow duplicate values
and elements can be modified.
</p>

<pre>
numbers = [1, 2, 3, 4]
numbers.append(5)
numbers.insert(1, 10)
numbers.remove(3)
print(numbers)
</pre>

<hr>

<h3>Tuple Data Type</h3>
<p>
A tuple is an ordered and immutable collection. Once created, elements cannot be changed.
Tuples are faster and safer for fixed data.
</p>

<pre>
t = (10, 20, 30)
print(t[0])
print(len(t))
</pre>

<hr>

<h3>Set Data Type</h3>
<p>
A set is an unordered collection of unique elements. Duplicate values are automatically removed.
</p>

<pre>
s = {1, 2, 3, 3, 4}
s.add(10)
print(s)
</pre>

<h4>Set Operations</h4>
<pre>
a = {1, 2, 3}
b = {3, 4, 5}
print(a.union(b))
print(a.intersection(b))
</pre>

<hr>

<h3>Dictionary Data Type</h3>
<p>
A dictionary stores data in key-value pairs. Keys must be unique and immutable.
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

<hr>

<h2>Type Conversion</h2>
<p>
Type conversion is the process of converting one data type into another.
</p>

<h3>Implicit Type Conversion</h3>
<pre>
x = 10
y = 2.5
z = x + y
print(z)
print(type(z))
</pre>

<h3>Explicit Type Conversion</h3>
<pre>
a = "100"
b = int(a)
print(b + 20)
</pre>

<hr>

<h2>Python Operators</h2>

<h3>Arithmetic Operators</h3>
<pre>
a = 10
b = 3
print(a + b)
print(a - b)
print(a * b)
print(a / b)
print(a % b)
</pre>

<h3>Assignment Operators</h3>
<pre>
x = 5
x += 2
x *= 3
print(x)
</pre>

<h3>Comparison Operators</h3>
<pre>
a = 10
b = 20
print(a == b)
print(a < b)
print(a != b)
</pre>

<h3>Logical Operators</h3>
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
Loops are used to repeat a block of code multiple times.
</p>

<h3>for Loop</h3>
<pre>
for i in range(1, 6):
    print(i)
</pre>

<h3>while Loop</h3>
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
Functions are reusable blocks of code used to perform specific tasks.
They help reduce code repetition.
</p>

<h3>Defining a Function</h3>
<pre>
def greet():
    print("Hello Python")

greet()
</pre>

<h3>Function with Parameters and Return</h3>
<pre>
def add(a, b):
    return a + b

result = add(10, 20)
print(result)
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
Lambda functions are small anonymous functions written in one line.
</p>

<pre>
square = lambda x: x * x
print(square(5))
</pre>

<hr>

<h2>File Handling</h2>
<p>
File handling allows reading and writing data to files.
</p>

<pre>
file = open("sample.txt", "w")
file.write("Hello Python")
file.close()

file = open("sample.txt", "r")
print(file.read())
file.close()
</pre>

<hr>

<h2>Final Conclusion</h2>
<p>
This document provides a complete and detailed explanation of Python fundamentals,
including variables, data types, operators, loops, functions, lambda expressions,
and file handling with practical examples. These concepts build a strong foundation
for advanced Python programming.
</p>
