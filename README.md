<h1>Python Fundamentals</h1>

<hr>

<h2>Python Variables</h2>
<p>
A variable is a container used to store data values in memory. In Python, variables are created automatically
when a value is assigned to them. Python is a dynamically typed language, meaning you do not need to
declare the data type of a variable explicitly.
</p>

<p>
Variables make programs flexible and readable by allowing data to be reused and modified easily.
</p>

<h3>Rules for Naming Variables</h3>
<ul>
  <li>Variable names must begin with a letter (A–Z or a–z) or an underscore (_).</li>
  <li>They cannot start with a number.</li>
  <li>They may contain letters, numbers, and underscores only.</li>
  <li>Variable names are case-sensitive (for example, <code>age</code> and <code>Age</code> are different).</li>
  <li>Python keywords (like <code>if</code>, <code>for</code>, <code>while</code>) cannot be used as variable names.</li>
</ul>

<pre>
x = 10
name = "Python"
_total = 50
</pre>

<p>
In the above example, <code>x</code> stores a number, <code>name</code> stores a string,
and <code>_total</code> stores another numeric value.
</p>

<hr>

<h2>Python Data Types</h2>
<p>
Data types specify the kind of value a variable holds. Python supports several built-in data types
to handle different kinds of data efficiently.
</p>

<h3>Numeric Data Types</h3>
<p>
Numeric data types are used to store numbers.
</p>
<ul>
  <li><b>int</b>: Stores whole numbers without decimals.</li>
  <li><b>float</b>: Stores numbers with decimal points.</li>
  <li><b>complex</b>: Stores numbers with real and imaginary parts.</li>
</ul>

<pre>
a = 10
b = 3.5
c = 2 + 4j
</pre>

<p>
Here, <code>a</code> is an integer, <code>b</code> is a floating-point number, and <code>c</code> is a complex number.
</p>

<hr>

<h3>String Data Type</h3>
<p>
A string is a sequence of characters enclosed within single quotes or double quotes.
Strings are commonly used to store text data.
</p>

<pre>
text = "Hello Python"
print(text[0])
print(text[-1])
print(text[0:5])
</pre>

<p>
Strings support indexing and slicing, which allows access to individual characters or parts of the string.
</p>

<h4>Common String Methods</h4>
<ul>
  <li><b>upper()</b>: Converts text to uppercase.</li>
  <li><b>lower()</b>: Converts text to lowercase.</li>
  <li><b>strip()</b>: Removes leading and trailing spaces.</li>
  <li><b>replace()</b>: Replaces characters or words.</li>
  <li><b>split()</b>: Splits a string into a list.</li>
</ul>

<pre>
s = " python "
print(s.strip())
print(s.upper())
</pre>

<hr>

<h3>List Data Type</h3>
<p>
A list is an ordered and mutable collection of elements. Lists allow duplicate values
and elements can be changed after creation.
</p>

<pre>
nums = [1, 2, 3, 4]
nums.append(5)
nums[0] = 10
print(nums)
</pre>

<p>
Lists are widely used to store multiple values in a single variable.
</p>

<h4>Common List Operations</h4>
<ul>
  <li><b>append()</b>: Adds an element at the end.</li>
  <li><b>insert()</b>: Inserts an element at a specific position.</li>
  <li><b>remove()</b>: Removes a specific element.</li>
  <li><b>pop()</b>: Removes an element by index.</li>
  <li><b>sort()</b>: Sorts the list.</li>
</ul>

<hr>

<h3>Tuple Data Type</h3>
<p>
A tuple is similar to a list but is immutable, meaning its elements cannot be changed
after creation. Tuples are useful when data should remain constant.
</p>

<pre>
t = (10, 20, 30)
print(t[1])
</pre>

<hr>

<h3>Set Data Type</h3>
<p>
A set is an unordered collection of unique elements. Duplicate values are automatically removed.
Sets are useful for mathematical operations like union and intersection.
</p>

<pre>
s = {1, 2, 3, 3, 4}
print(s)
</pre>

<h4>Common Set Operations</h4>
<ul>
  <li><b>add()</b>: Adds an element.</li>
  <li><b>remove()</b>: Removes an element.</li>
  <li><b>union()</b>: Combines two sets.</li>
  <li><b>intersection()</b>: Finds common elements.</li>
</ul>

<hr>

<h3>Dictionary Data Type</h3>
<p>
A dictionary stores data in key–value pairs. It is used when data needs to be associated
with unique keys.
</p>

<pre>
student = {
  "name": "Ravi",
  "age": 21,
  "course": "Python"
}
print(student["name"])
</pre>

<p>
Dictionaries are widely used for structured data representation.
</p>

<hr>

<h2>Type Conversion</h2>
<p>
Type conversion refers to changing one data type into another. Python supports both implicit
and explicit type conversion.
</p>

<h3>Implicit Conversion</h3>
<p>
Python automatically converts one data type into another when no data loss occurs.
</p>

<pre>
a = 10
b = 2.5
c = a + b
print(c)
</pre>

<h3>Explicit Conversion</h3>
<p>
Explicit conversion is done manually using built-in functions.
</p>

<pre>
x = "100"
y = int(x)
print(y + 10)
</pre>

<hr>

<h2>Python Operators</h2>
<p>
Operators are symbols used to perform operations on variables and values.
</p>

<h3>Arithmetic Operators</h3>
<p>
Used to perform mathematical operations like addition, subtraction, multiplication, and division.
</p>

<h3>Comparison and Logical Operators</h3>
<p>
Comparison operators compare values, while logical operators combine multiple conditions
to produce a single result.
</p>

<h3>Membership and Identity Operators</h3>
<p>
Membership operators check for the presence of values, and identity operators compare
object memory locations.
</p>

<hr>

<h2>Loops</h2>
<p>
Loops are used to repeat a block of code multiple times. They reduce redundancy
and make programs efficient.
</p>

<h3>for Loop</h3>
<p>
The for loop is used to iterate over sequences like lists, strings, and ranges.
</p>

<h3>while Loop</h3>
<p>
The while loop executes code as long as a condition remains true.
</p>

<h3>Loop Control Statements</h3>
<p>
Statements like <b>break</b>, <b>continue</b>, and <b>pass</b> control the flow of loops.
</p>

<hr>

<h2>Functions</h2>
<p>
Functions are reusable blocks of code that perform a specific task. They improve
modularity and readability of programs.
</p>

<h3>Parameters and Return Values</h3>
<p>
Functions can accept input parameters and return output using the <b>return</b> statement.
</p>

<hr>

<h2>Lambda Functions</h2>
<p>
Lambda functions are anonymous functions written in a single line.
They are useful for short, simple operations.
</p>

<hr>

<h2>File Handling</h2>
<p>
File handling allows Python programs to read from and write to files.
This is essential for data storage and retrieval.
</p>

<hr>

<h2>Final Conclusion</h2>
<p>
This document explains Python fundamentals in detail, covering variables, data types,
type conversion, operators, loops, functions, lambda expressions, and file handling.
These concepts form a strong foundation for advanced Python programming and real-world applications.
</p>
