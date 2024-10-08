# **Root Finding**

This project is a web application built firstly in C++ and than translated to HTML ans JS for hosting reasons.

Project Uses Four different root finding algorithms: Bisection method, Fixed point method, Newton method and combination of Bisection and Newton method.

## **How to use it and what it does**

**How to use it**

This project can find the root to any powered polynomial if given enough time and not awful initial guesses (For example: x^2 + x - 4 = 0). 

You need to input firstly l (lower bound) and r (upper bound), the initial guess of x, the highest power of x and coefficients of each variable from (x^0 + ... +x^n) in this polynomial.

**What it does**

For each of the methods if it finds the answer it will give us the answer itself and how many itterations it needs.

Also it will give us two graphs, first one shows itterations by graph and second one shows the distance between final answer (if found) and guessed number for each itteration.


## **How to access it**

**First Way**

You can just follow this link to access this code.

```bash
https://rootfinding.tiiny.site/
```

**Second Way**

You can clone repository using:
```bash
https://github.com/Mate-ber/Root-Finding-Project.git
```
 After downloading just simply host it locally.

**Third way**

You can simply download the file and just run it locally.

## **Little bit about each algorithm**

**Bisection Method**

Bisection Method wors by repeatedly dividing an interval in half and selecting the subinterval, where the function changes sign (indicating a root exists in that interval).

The process continues until the interval is sufficiently small.

(BE AWARE) This method guarantees convergence if answe is in given interval but can be slow.

**Fixed point method***

It starts with an initial guess and applies the function repeatedly x(n+1) = g(x(n)), hoping the sequence converges to a point where x=g(x) which is fixed point.

(BE AWARE) It won't find the answer always cause it requires function g(x) to satisfy certain conditions (like being a contraction) to ensure convergence.

**Newton method**

Starting from an initial guess, it uses the formula x(n+1) = x(n) - f(x(n))/ f'(x(n)), where f'(x(n)) is the derivative of the function f(x(n)).

(BE AWARE) Newton's method converges quickly when close to the root but can fail if the initial guess is far from the root or if the derivative is zero.

**Bisection + Newton method**

This hybrid approach uses always the solvability of the Bisection method and the speed of Newton's method.

Initially, the Bisection method is used to narrow down the interval containing the root.

Once the interval is sufficiently small or a good initial guess is found, Newton's method is applied for rapid convergence.

This method combines the strengths of both algorithms: the guaranteed convergence of Bisection and the efficiency of Newton's method.

In most cases the best method.
