## Adaptive Routing for Network Overload Avoidance using Genetic Algorithm

### Design and implement a genetic algorithm based route optimization algorithm to identify fastest route in a network with dynamic values of latency and jitter.

Each ‘route’ object is a chromosome
The chromosome (route) is a linked list of routers (Router Objects). 
Each router in the route points to the next router in sequence

Each ‘router’ object represents a gene in the chromosome. 
Each gene includes : 
1. IP Address 
2. Last Octet
3. Latency to next router
4. jitter
5. Fitness Value

### Fitness Function 

Higher Fitness means: 

1. Lower Latency
2. Stable Jitter
3. Shorter total time of route


### Other Functions used 

1. remove_repeated 
2. detect_repeated
3. mount_route
4. update_total_latencies
5. count_routers
6. evaluate_fitness
7. collect_generations_history
8. run_generations

## Comparing GA and Dijkstra's Algorithm 

#### Optimizing for Multiple Objectives:
##### GA can be used to optimize for multiple objectives simultaneously, such as minimizing time, energy consumption, or load balancing.
#### Exploration of Solution Space:
##### GA explores a wide solution space whereas  Dijkstra's will converge to a optimum value. 

##### Genetic Algorithms are adaptable to dynamic or changing network conditions. 
##### GA can discover and optimize multiple routes, enabling load balancing across the network.
##### Helpful in scenarios where distributing traffic or resources across multiple paths is essential for efficiency and reliability.

##### Dijkstra's algorithm would requires less memory compared to genetic algorithm.
##### Dijkstra's algorithm guarantees an optimal solution for finding the shortest path in a weighted graph. It finds the globally optimal solution in terms of the sum of edge weights.
##### Dijkstra's algorithm is highly efficient for solving single-objective shortest path problems.
##### Genetic Algorithms involve randomness in the initialization and evolution processes, leading to different results in different runs.

