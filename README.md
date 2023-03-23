# Project 1 - Gradient Descent Methods\n,


$\mathbf{Goal: }$ To solve the optimal control problem,
$$ \min_{u \in L^2(\Omega)} J(Y,u) = \frac{1}{2} || y - y_d||^2 + \frac{\gamma}{2} || u ||^2$$,
$$ \text{subject to } \begin{cases} -\Delta y = u , & \text{in } \Omega \\\\ y \\big|_{\\partial \\Omega } = 0 ,& \\text{on } \\partial \\Omega \\end{cases}$$\n,
\n,
Let $Su = y \\Rightarrow f'(u) = S^*(Su - y_d) + \\gamma u$, then we have the KKT system:\n,
- State problem: \n,
$$ \\begin{cases} -\\Delta y = u , & \\text{in } \\Omega \\\\ y  = 0 ,& \\text{on } \\partial \\Omega \\end{cases}$$\n,
- Adjoint problem:\n,
$$ \\begin{cases} -\\Delta p = y - y_d , & \\text{in } \\Omega \\\\ p = 0 ,& \\text{on } \\partial \\Omega \\end{cases}$$\n,
- Optimality condition:
$$ p + \gamma u = 0$$
 
 
The report presents 3 optimization methods to solve this optimal control problem:,
1. Steepest gradient descent with Amijo search for step-size $\alpha$,
2. Steepest gradient descent with exact search for step-size $\alpha$,
3. Conjugate gradient descent
