<h1>Python Fundamentals</h1>
<p>This document explains Python data types, variables, rules, type conversion, operators, and core built-in data structures such as <b>String, List, Tuple, Set, and Dictionary</b>. Each topic is explained in detail with clear examples.</p>

<hr>

<h2>1. Python Variables</h2>
<p>A variable is a name used to store data in memory. Python does not require explicit declaration of variable types.</p>

<h3>Rules for Naming Variables</h3>
<ul>
  <li>Must start with a letter (a-z, A-Z) or underscore (_)</li>
  <li>Cannot start with a number</li>
  <li>Can contain letters, numbers, and underscores</li>
  <li>Case-sensitive (age and Age are different)</li>
  <li>Cannot use Python keywords</li>
</ul>

<h3>Examples</h3>
<pre>
x = 10
name = "Python"
_total = 50
</pre>

<hr>

<h2>2. Python Data Types</h2>
<p>Data types define the type of value stored in a variable.</p>

<h3>2.1 Numeric Data Types</h3>
<ul>
  <li><b>int</b> – Whole numbers</li>
  <li><b>float</b> – Decimal numbers</li>
  <li><b>complex</b> – Numbers with real and imaginary parts</li>
</ul>

<pre>
a = 10
b = 3.5
c = 2 + 4j
</pre>

<hr>

<h3>2.2 String Data Type</h3>
<p>Strings are sequences of characters enclosed in single or double quotes.</p>

<pre>
text = "Hello Python"
print(text[0])       # H
print(text[-1])      # n
print(text[0:5])     # Hello
</pre>

<h4>Common String Methods</h4>
<ul>
  <li>upper()</li>
  <li>lower()</li>
  <li>strip()</li>
  <li>replace()</li>
  <li>split()</li>
</ul>

<pre>
s = " python "
print(s.strip())
print(s.upper())
</pre>

<hr>

<h3>2.3 List Data Type</h3>
<p>Lists are ordered, mutable collections that allow duplicate values.</p>

<pre>
nums = [1, 2, 3, 4]
nums.append(5)
nums[0] = 10
print(nums)
</pre>

<h4>Common List Operations</h4>
<ul>
  <li>append()</li>
  <li>insert()</li>
  <li>remove()</li>
  <li>pop()</li>
  <li>sort()</li>
</ul>

<hr>

<h3>2.4 Tuple Data Type</h3>
<p>Tuples are ordered and immutable collections.</p>

<pre>
t = (10, 20, 30)
print(t[1])
</pre>

<h4>Tuple Use Case</h4>
<p>Used when data should not be changed.</p>

<hr>

<h3>2.5 Set Data Type</h3>
<p>Sets are unordered collections with unique elements.</p>

<pre>
s = {1, 2, 3, 3, 4}
print(s)
</pre>

<h4>Set Operations</h4>
<ul>
  <li>add()</li>
  <li>remove()</li>
  <li>union()</li>
  <li>intersection()</li>
</ul>

<hr>

<h3>2.6 Dictionary Data Type</h3>
<p>Dictionaries store data in key-value pairs.</p>

<pre>
student = {
  "name": "Ravi",
  "age": 21,
  "course": "Python"
}
print(student["name"])
</pre>

<h4>Dictionary Methods</h4>
<ul>
  <li>keys()</li>
  <li>values()</li>
  <li>items()</li>
  <li>get()</li>
</ul>

<hr>

<h2>3. Type Conversion (Type Casting)</h2>
<p>Type conversion is converting one data type into another.</p>

<h3>Implicit Conversion</h3>
<pre>
a = 10
b = 2.5
c = a + b
print(c)
</pre>

<h3>Explicit Conversion</h3>
<pre>
x = "100"
y = int(x)
print(y + 10)
</pre>

<h4>Common Conversion Functions</h4>
<ul>
  <li>int()</li>
  <li>float()</li>
  <li>str()</li>
  <li>list()</li>
  <li>tuple()</li>
  <li>set()</li>
</ul>

<hr>

<h2>4. Python Operators</h2>

<h3>4.1 Arithmetic Operators</h3>
<pre>
a = 10
b = 3
print(a + b)
print(a - b)
print(a * b)
print(a / b)
print(a % b)
</pre>

<h3>4.2 Assignment Operators</h3>
<pre>
x = 5
x += 2
x -= 1
</pre>

<h3>4.3 Comparison Operators</h3>
<pre>
a = 10
b = 20
print(a == b)
print(a != b)
print(a < b)
</pre>

<h3>4.4 Logical Operators</h3>
<pre>
a = True
b = False
print(a and b)
print(a or b)
print(not a)
</pre>

<h3>4.5 Membership Operators</h3>
<pre>
nums = [1, 2, 3]
print(2 in nums)
print(5 not in nums)
</pre>

<h3>4.6 Identity Operators</h3>
<pre>
a = 10
b = 10
print(a is b)
print(a is not b)
</pre>

<hr>

<h2>5. print() Function</h2>
<p>The <b>print()</b> function is used to display output.</p>

<pre>
name = "Python"
age = 10
print("Language:", name)
print(f"Age: {age}")
</pre>

<hr>

<h2>Conclusion</h2>
<p>This document covers Python variables, data types, built-in collections, type conversion, and operators with practical examples. These concepts form the foundation for advanced Python programming.</p>
```

