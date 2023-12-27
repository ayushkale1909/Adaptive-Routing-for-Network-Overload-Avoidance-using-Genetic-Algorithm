# Adaptive Routing for Network Overload Avoidance using Genetic Algorithm

## Design and implement a genetic algorithm based route optimization algorithm to identify fastest route in a network with dynamic values of latency and jitter.

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

## Fitness Function 

Higher Fitness means: 

1. Lower Latency
2. Stable Jitter
3. Shorter total time of route


## Functions used 

remove_repeated 
detect_repeated
mount_route
update_total_latencies
count_routers
evaluate_fitness
collect_generations_history
run_generations
