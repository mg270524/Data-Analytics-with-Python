Q3. Write a python programme (UDF) to input three real numbers a,b and c 
and check if it forms a triange. If so find the nature of the triangle 
and hence print its area using the Heron's formula.

```python
from math import sqrt

a = int(input("Enter a number."))
b = int(input("Enter a number."))
c = int(input("Enter a number."))

def check_tri():
    if a+b>c and b+c>a and a+c>b:
        print ("The three numbers form a triangle.")
    else:
        print("The three numbers do not form a triangle.")
check_tri()

def area_tri():
    s = (a+b+c)/2
    area = sqrt(s*(s-a)*(s-b)*(s-c))
    print(f"The area of the triangle is {area}")
area_tri()

```

Q4. Write a python programme (UDF) to find the root of an equation f(x) = 0 
using the bisection method and hence use your defined function to find the 
root of a cubic $ax^3 + bx^2 + cx + d = 0$ in an appropriate domain.

Q5. Write a python programme to find the approximate value of pi 
using the Monte Carlo method.

Q6. Write a python programme to estimate the value of log(a) for any 
positive real numbers a using the Mclautrin series expansion\

Q7. write a python programme to find roots of a depressed cubic $x^3 + px + q = 0$
by considering all possible cases.
