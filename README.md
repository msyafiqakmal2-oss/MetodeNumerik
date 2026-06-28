# MetodeNumerik

Assigment From Pak Oddy
def f(x):
    return x 3 - x - 2

def bisection(a, b, error=0.0001):
    if f(a) * f(b) >= 0:
        print("Nilai a dan b tidak memenuhi syarat")
        return 

    while (b - a) / 2 > error:
        c = (a + b) / 2
        if f(c) == 0:
            return c
        elif f(a) * f(c) < 0:
            b = c
        else:
            a = c

    return (a + b) / 2

print("Akar:", bisection(1, 2))

Numerical Methods (Metode Numerik) are a branch of Mathematics that focuses on solving problems using approximation techniques instead of exact analytical solutions. These methods are especially important when problems are too complex to solve using standard formulas or symbolic manipulation.

In simple terms, numerical methods are are tep-by-step computational procedures used to find approximate solutions to mathematical problems. Instead of solving equations exactly (like in algebra), we use algorithms that produce close enough answers.

This approach is heavily used in Computer Science, engineering, physics, and data science because real-world problems often involve:

> Complicated equations
> Large datasets
> Nonlinear relationships
> Systems that cannot be solved analytically

Why Do We Need Numerical Methods?

Many mathematical problems cannot be solved using exact formulas. For example:

> Finding roots of nonlinear equations
> Solving large systems of equations
> Integrating functions that have no closed-form solution
> Simulating real-world systems (weather, traffic, economics)

Numerical methods allow computers to approximate solutions efficiently using algorithms. and good
