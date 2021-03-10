# Class Reference

## GeneticAlgorithm

### Parameters

* **chromosome** - object of a custom class, the reason for this is so some additional stuff related to fitness function may be designed

* **params** - a dict containing GA parameters displayed in the 'defaults' variable

* **args** - tuple('int'/'float', list of tuples defining limits for chromosome parameters), tuple('string', number_of_args), tuple('bool', number_of_args)
fitness_function - handle to a fitness function that needs   to be a class function of chromosome object's class

### Class Attributes  

* `defaults` - A dictionary which holds the default values for various components requied by the algorithm.

  * `pop_size` - 

  * `relative_tolerance` - if difference between two gen is smaller than this parameter, the algorithm stops

  * `absolute_tolerance` - if gen fitness score is bigger than this, algorithm stops

  * `best_member_fitness_stop_condition` - if this is a float, when one of the solutions in the GA surpasses the value, the algorithm terminates

  * `selection` - best members still get to the next generation, but all are favored instead of just top N determined by elitism

  * `elitism_threshold` - how many of the best chromosomes get to be kept in the population

  * `elitism_trigger` - when average generation fitness reaches float value for triggers, it switches to another selection

  * `ranked_trigger` - 

  * `ranked_rank_probability` - splits population into len(arg) parts, then assigns each rank probability equal to index list member

  * `proportional_trigger` - 

  * `mutation_rate` - 

  * `mutation_repeats` - how many mutations per chromosome (same genes may mutate multiple times)

  * `mutation_intensity` - for float/int representation (maximum possible offset when mutating)

  * `max_iter` - max iterations before algorithm stops

  * `seed` - 

  * `prop_trig` - 

  * `ranked_trig` - 

  * `char_list` - char list that limits string representation chromosome states

  * `keep_parents_during_crossover` - let parents crossover into next generation

  * `number_of_safe_gens` - number of gens before stop conditions start to apply

  * `filter_return` - if this value is true, GA only returns chromosomes >= of 'filter_threshold'

  * `filter_threshold` - 