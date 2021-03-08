# Class Reference

## GeneticAlgorithm

* **chromosome** - object of a custom class, the reason for this is so some additional stuff related to fitness function may be designed

* **params** - a dict containing GA parameters displayed in the 'defaults' variable

* **args** - tuple('int'/'float', list of tuples defining limits for chromosome parameters), tuple('string', number_of_args), tuple('bool', number_of_args)
fitness_function - handle to a fitness function that needs to be a class function of chromosome object's class

## Chromosone
