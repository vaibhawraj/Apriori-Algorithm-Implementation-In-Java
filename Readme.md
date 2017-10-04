Java Implementation of Apriori Algorithm
==========================================


The code attempts to determine the list of frequent item set using Apriori Algorithm. Any item set is said to be frequent if support for that item set is greater than minimum support threshold.

Input format
-------

Program excepts input from standard input or via file redirection. Input format is:

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
    
    
 