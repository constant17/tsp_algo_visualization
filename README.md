# Traveling Salesman Problem

![Klip video April 4th 2024 11_57 am](https://github.com/constant17/tsp_algo_visualization/assets/29698810/459052f3-1038-49a7-811a-2808073bdab0)


The traveling salesman problem (TSP) is a very known optimization problem that seeks to solve the following challenge: given a set of cities and a cost to travel from one city to another, identify the route that will allow a salesman to visit each city at the minimum cost and only once, starting and ending in the same city.

### This project

- Live at 

- For example, apply nearest neighbor, then 2-opt inversion, then branch and bound

### Heuristic algorithms

Heuristic algorithms attempt to find a good approximation of the optimal path within a more _reasonable_ amount of time.

**Construction** - Build a path

- Nearest Neighbor
- Arbitrary Insertion
- Furthest Insertion
- Nearest Insertion
- Convex Hull Insertion\*
- Simulated Annealing\*

**Improvement** - Attempt to take an existing constructed path and improve on it

- 2-Opt Reciprocal Exchange
- 2-Opt Inversion\*

### Exhaustive algorithms

Exhaustive algorithms will always find the best possible solution by evaluating every possible path. These algorithms are typically significantly more expensive then the heuristic algorithms discussed above. The exhaustive algorithms implemented so far include:

- Random Paths
- Depth First Search (Brute Force)
- Branch and Bound (Cost)
- Branch and Bound (Cost, Intersections)\*

## Dependencies

These are the main tools used to build this site:

- [gatsbyjs](https://www.gatsbyjs.org)
- [reactjs](https://reactjs.org)
- [web workers](https://developer.mozilla.org/en-US/docs/Web/API/Web_Workers_API)
- [material-ui](https://material-ui.com/)
- [deck.gl](https://deck.gl/#/)
- [mapbox](https://www.mapbox.com/)

## Contributing

Pull requests are always welcome! Also, feel free to raise any ideas, suggestions, or bugs as an issue.
