## [Optimization](https://en.wikipedia.org/wiki/Mathematical_optimization)

### Problem Formation

* Decision Variables: describe the state of a system
* [Loss/Cost/Objective Function](https://en.wikipedia.org/wiki/Loss_function): assess the state of a system
  * [Maxima and Minima](https://en.wikipedia.org/wiki/Maxima_and_minima)
    * Global Maxima and Minima vs. Local Maxima and Minima

![Local and global maxima and minima for cos(3πx)/x, 0.1≤ x ≤1.1](https://upload.wikimedia.org/wikipedia/commons/6/68/Extrema_example_original.svg)

* Constraints
  * Transformations
    * x = x⁺ + 1
    * min{f(x} = -max{-f(x)}
    * x < 0 -> -x > 0
    * x = 0 -> 0 <= x and x >= 0
    * x = x⁺ + x⁻
    * x <= u -> x - u <= 0
    * [Slack Variables](https://en.wikipedia.org/wiki/Slack_variable)

### [Convex Optimization](https://en.wikipedia.org/wiki/Convex_optimization)

* [Duality](https://en.wikipedia.org/wiki/Duality_(optimization))
  * [Lagrangian](https://en.wikipedia.org/wiki/Lagrange_multiplier)
    * [Karush–Kuhn–Tucker Conditions](https://en.wikipedia.org/wiki/Karush–Kuhn–Tucker_conditions)

### Unconstrained vs. Constrained Optimization

* Unconstrained Optimization
  * [Conjugate Gradient Method](https://en.wikipedia.org/wiki/Conjugate_gradient_method)
  * [Newton's Local Method](https://en.wikipedia.org/wiki/Newton%27s_method): find solution to ∇f(x) = 0
  * [Gradient Descent](https://en.wikipedia.org/wiki/Gradient_descent)
* [Constrained Optimization](https://en.wikipedia.org/wiki/Constrained_optimization)

### Continious vs. Discrete Optimization

* [Continious Optimization](https://en.wikipedia.org/wiki/Continuous_optimization)
  * [Lipschitz Continuity](https://en.wikipedia.org/wiki/Lipschitz_continuity)
* [Discrete Optimization](https://en.wikipedia.org/wiki/Discrete_optimization)
  * [Integer](https://en.wikipedia.org/wiki/Integer_programming) [Linear Programming](https://en.wikipedia.org/wiki/Linear_programming)
    * [Simplex algorithm](https://en.wikipedia.org/wiki/Simplex_algorithm)
  * [Combinational Optimization](https://en.wikipedia.org/wiki/Combinatorial_optimization)
    * [Graphs](https://en.wikipedia.org/wiki/Graph_(discrete_mathematics))
      * [Vehicle Routing Problem](https://en.wikipedia.org/wiki/Vehicle_routing_problem)
        * Least Cost Path
          * [Dijkstra's Algorithm](https://en.wikipedia.org/wiki/Dijkstra%27s_algorithm)
          * [A* Search Algorithm](https://en.wikipedia.org/wiki/A*_search_algorithm)
      * [Traveling Salesman Problem](https://en.wikipedia.org/wiki/Travelling_salesman_problem)
    * [Minimum Spanning Tree](https://en.wikipedia.org/wiki/Minimum_spanning_tree)

### [Differentiable](https://en.wikipedia.org/wiki/Differentiable_function) vs. Nondifferentiable Optimization

* Differentiable Optimization
  * [Newton's Method](https://en.wikipedia.org/wiki/Newton%27s_method_in_optimization)
  * [Gradient Descent](https://en.wikipedia.org/wiki/Gradient_descent)
  * nice properties to have
    * [Linearity](https://en.wikipedia.org/wiki/Linearity)
    * [Affinity](https://en.wikipedia.org/wiki/Affine_transformation)

### Deterministic vs. [Stochastic Optimization](https://en.wikipedia.org/wiki/Stochastic_optimization)

* Stochastic Optimization
  * [Stochastic Gradient Descent](https://en.wikipedia.org/wiki/Stochastic_gradient_descent)
  * [Simultaneous perturbation stochastic approximation](https://en.wikipedia.org/wiki/Simultaneous_perturbation_stochastic_approximation)

### References

* [Northwestern University Open Text Book on Process Optimization](https://optimization.mccormick.northwestern.edu/index.php/Main_Page) [optimization.mccormick.northwestern.edu]
* [Optimization@MIT](http://optimization.mit.edu/classes.php) [optimization.mit.edu]
* [Optimization: principles and algorithms, by Michel Bierlaire](http://optimizationprinciplesalgorithms.com) [optimizationprinciplesalgorithms.com]

### Other
* [No Free Lunch](https://en.wikipedia.org/wiki/No_free_lunch_in_search_and_optimization)
* [Pareto efficiency](https://en.wikipedia.org/wiki/Pareto_efficiency)
* Exploration vs Exploitation
  * Greedy: always choose highest value, but gets stuck easily
  * Non-Greedy: may choose a non-optimal solution
* [Dynamic programming](https://en.wikipedia.org/wiki/Dynamic_programming)


