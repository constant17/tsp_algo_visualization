# Animated Visualization of the Algorithms Solving the Traveling Salesman Problem

The traveling salesman problem (TSP) is a very well-known optimization problem that seeks to solve the following challenge: given a set of cities and a cost to travel from one city to another, identify the route that will allow a salesman to visit each city at the minimum cost and only once, starting and ending in the same city. <br />
Below is a screen recording of the application showing an animated visualization of [Convex Hull algorithm](https://en.wikipedia.org/wiki/Convex_hull_algorithms) solving the TSP problem.
<br /> <br />
![Klip video April 4th 2024 11_57 am](https://github.com/constant17/tsp_algo_visualization/assets/29698810/459052f3-1038-49a7-811a-2808073bdab0)


## Requirements
- NodeJS -v 16.x.x
- This project uses `remark-mdx` package, which only works with NodeJS 16.

##  Local Installation

- Fork or download the project
- Move to the root directory of the project and run `npm install`
- Run `npm run develop` or `npm start` to launch the project. It should run on port 8000 if it's available so open the browser with `http://localhost:8000/`


## [Solutions to the TSP problem](https://optimization.cbe.cornell.edu/index.php?title=Traveling_salesman_problem)

#### Exact algorithms
The most straightforward algorithmic solution is a complete enumeration of all possible paths to determine the path of least cost. Thus, for `n` cities, the algorithm performs in
`O(n!)` time, and this method is practical only for extremely small values of `n`.
Branch-and-bound algorithms are also used to find solutions for the TSP problem. 

Other exact solution methods include the [cutting plane](https://en.wikipedia.org/wiki/Cutting-plane_method) method and [branch-and-cut](https://en.wikipedia.org/wiki/Branch_and_cut).

#### Heuristic algorithms
The TSP is considered an NP-hard problem so heuristic algorithms are used to give approximate solutions that are good, though not necessarily optimal. The algorithms do not guarantee an optimal solution, but gives near-optimal solutions in reasonable computational time.3 The Held-Karp lower bound can be calculated and used to judge the performance of a heuristic algorithm.3

There are two general [heuristic classifications](http://i.stanford.edu/pub/cstr/reports/cs/tr/85/1066/CS-TR-85-1066.pdf)

* Tour construction procedures where a solution is gradually built by adding a new vertex at each step
* Tour improvement procedures where a feasbile solution is improved upon by performing various exchanges
The best methods tend to be composite algorithms that combine these features

## Implemented Algorithms  to Find the Shortest Path
#### Heuristic algorithms

- Nearest Neighbor
- Arbitrary Insertion
- Furthest Insertion
- Nearest Insertion
- Convex Hull Insertion\*
- Simulated Annealing\*

**Improvement** - Attempt to take an existing constructed path and improve on it

- 2-Opt Reciprocal Exchange
- 2-Opt Inversion\*

#### Exhaustive algorithms

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
