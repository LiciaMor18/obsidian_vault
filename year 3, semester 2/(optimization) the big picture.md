## flows in graphs
we started by covering *flows in graphs*.
we defined *networks* and *flows* (which are functions on edges, with certain properties)
we proved the *conservation of flow* property and defined the *value of a flow*
we defined *realgorithm sidual graphs* and used them to define a *flow-augmenting path* given by a residual graph, and used it to make a new function which is a *flow*. (in practice, defined how to add to a graph)

we studied the *ford-fulkerson algorithm*  (*FF*) and showed that it always terminates if the capacities are integers
to certify the optimality of the ford-fulkerson algorithm, we introduced *st-cuts*. they give an upper bound to the optimal flow of a graph.
- furthermore, we can find a st-cut that matches the max flow value given by the FF algorihtm, certifying its optimality

as the FF algorithm runs in exponential time, we introduce the *Elmands + Karp algorithm* (*EK*), that terminates in polinomial time even with real-valued capacities.
- the EK algorithm is just like the FF algorithm, but it takes the shortest $s \to t$ path in the residual graph (finds it using a BFS)
we proved EK algorithms’s upper bound on steps ($n\cdot m$)

## linear programs
we introduced the structure of *linear programs*
we studied that a linear program has either:
1) a unique optimal solution
2) infinitely many optimal solutions
3) no feasible solutions
4) a feasible solution but no optimal solution (unbounded)

we studied *convex* feasible sets
- we proved that all linear programs have a convex feasible set
- 
### geometry
we first noticed that the objective function can be re-written as a scalar product, and its gradient (the coefficients) point to the directions of steepest increase
## integer problems
