# MetodeNumerik

Assigment From Pak Oddy
def f(x):
    return x**3 - x - 2

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
