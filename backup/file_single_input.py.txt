import math

with open('input_single.txt', 'r') as f:
    a = float(f.readline())
    b = float(f.readline())
    c = float(f.readline())

D = b**2 - 4*a*c
if D >= 0:
    x1 = (-b + math.sqrt(D)) / (2*a)
    x2 = (-b - math.sqrt(D)) / (2*a)
    print("Roots are:", x1, x2)
else:
    print("No real roots")
