Activity 4: Exploring Calculus with SymPy
Objective:
This activity introduces basic concepts of calculus using the Python library SymPy, helping learners explore symbolic algebra, limits, derivatives, series expansion, and equation solving — all without manually solving complex math.

1. Playing with Symbols
What does x + x mean?
x + x is a symbolic expression. Since both terms are the same, the result simplifies to 2*x. This demonstrates SymPy's ability to apply algebraic rules just like traditional math.

What does x * x represent?
This represents x² (x squared). It shows that multiplying a symbol by itself correctly yields a power expression, which is fundamental in algebra and calculus.

2. Exploring Limits
What is the result of limit(sin(x)/x, x, 0)?
The result is 1. This limit is significant in calculus because although the expression sin(x)/x is undefined at x = 0, the limit exists and equals 1. It's a key example of how limits can be used to handle indeterminate forms.

3. Playing with Derivatives
What is the derivative of x²?
The derivative is 2*x. This tells us how fast the function x² changes with respect to x. In calculus terms, it's the slope of the tangent to the curve at any given point on the function.

4. Series Expansion
What do you see from the result of exp(x).series(x, 0, 4)?
The output shows the first few terms of the Taylor series expansion of the exponential function e^x. Specifically, the expansion includes:

1 (constant term)

x

x²/2

x³/6

This gives a polynomial approximation of e^x around x = 0.

5. Solving Equations
What are the solutions to x² - 4 = 0?
The solutions are [-2, 2]. These are the x-values where the quadratic equation intersects the x-axis — in other words, the roots of the equation.

What kind of problem is this?
This is a quadratic equation, involving a squared variable (x²) and solved by factoring or using algebraic methods to find the values of x that satisfy the equation.

6. Final Thoughts
What was your favorite part of the activity?
Using SymPy to compute limits and derivatives was the most engaging part. It helped make abstract calculus concepts more understandable and interactive.

What was something new or surprising you learned?
It was surprising to discover that Python, through SymPy, can handle algebra and calculus symbolically — returning exact expressions instead of just numerical approximations.