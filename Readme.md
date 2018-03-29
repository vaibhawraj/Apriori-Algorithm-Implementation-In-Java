Java Implementation of Apriori Algorithm
==========================================


The code attempts to determine the list of frequent item set using Apriori Algorithm. Any item set is said to be frequent if support for that item set is greater than minimum support threshold. It proceeds by identifying the frequent individual items in the database and extending them to larger and larger item sets as long as those item sets appear sufficiently often in the database. (Wiki on Apriori Algorithm)[https://en.wikipedia.org/wiki/Apriori_algorithm]

## Implementation
In order to keep it simple and understandable, implementation works on input in a particular format and processing it accordingly. That is by first determining sinlge item frequent set, and then using apriori property that any larger set of size K may be frequent if its all subset of k-1 size is also frequent. And thus reducing the search space and making it memory as well as time efficient algorithm.

Input format
-------

Program expects input from standard input or via file redirection. Input format is:

> First Line must contain positive integer greater than or equal to 2 which is Minimum Support Value
> 
> Second line onward, There should be comma separated list of items such that each line represents the list of item in particular transaction

For Example

	3
	apple,beer,rice,chicken
	apple,beer,rice
	apple,beer
	apple,mango
	milk,beer,rice,chicken
	milk,beer,rice
	milk,beer
	milk,mango

Output format
--------

Each line of output represents frequent item set with increasing number of size of item set

For Example

	apple
    beer
    rice
    milk
    apple, beer
    beer, rice
    beer, milk


Usage
-----
To compile the program on linux :

	$ make
    
To run the program

	$ java apriori < dataset/t01.dat
    
    
 
