## flows in graphs
we started by covering *flows in graphs*.
we defined *networks* and *flows* (which are functions on edges, with certain properties)
we proved the *conservation of flow* property and defined the *value of a flow*
we defined *realgorithm sidual graphs* and used them to define a *flow-augmenting path* given by a residual graph, and used it to make a new function which is a *flow*. (in practice, defined how to add to a graph)
we studied the *ford-fulkerson algorithm*  (*FF*) and showed that it always terminates if the capacities are integers

the certify the optimality of the ford-fulkerson algorithm, we introduced *st-cuts*. they give an upper bound to the optimal flow of a graph.
- furthermore, we can find a st-cut that matches the max flow value given by the FF algorihtm, certifying its optimality

## integer problems
