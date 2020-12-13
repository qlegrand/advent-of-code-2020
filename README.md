# advent-of-code-2020

So, I let myself be convinced to participate to de Advent of Code. I am starting late though. I intend to do my best to catch up, however I can't promise anything ;) 

The tasks are done in Python, as it is the language I am most comfortable with.

## [Day 1](https://adventofcode.com/2020/day/1)
The resolution of both problems come from recognising that the solution is the one that give multiple times the same result when we compute the product between a number in the list and it's complement to 2020.

More detailed explanations are available in the Notebook ;-)

## [Day 2](https://adventofcode.com/2020/day/2)

Somewhat not really challenging task as Python provides powerful methods to easily manage conditions on full lists. Main challenge was to parse the input file.

## [Day 3](https://adventofcode.com/2020/day/3)

Both problems of today are related to traversing matrixes with some predefined patterns and count elements that match some specific criteria. While problem 1 and problem 2 could have been resolved using the same method, I chose to explore 2 different, to spice things up ;-) .

What is given is a matrix with two kind of symbols. Problem statement says that this matrix can repeat itself horizontally an indefinite number of times if needed. Traversing the matrix is always done in the "go right x times, go down x times".

The first method relies on the regulatity of patterns and traversing. First I assign "0" to elements that don't need to be counted, "1" to elements that need to be counted. Then I manipulate the matrix to generate an equivalent square matrix that need to be traversed in the "R 1 D 1" fashion. Once we have that matrix, the trace of it is the anwer.

I thought to challenge a bit myself by coming up with the second method. First I assign "0" to elements that don't need to be counted, "1" to elements that need to be counted. Then the principle is to traverse the matrix up to down and left to right, applying the right modulo operator on the horizontal axis to circle the matrix correctly.

## [Day 4](https://adventofcode.com/2020/day/4)

Day 4 was a bit of a bummer. Main challenge was to load unformatted data into an array. From there, checking number of fields was trivial, and conditions allowed me to review a bit of Regex s*t 

## [Day 5](https://adventofcode.com/2020/day/5)
Problem was posed in an interesting way. Once I understood that decoding was direct from initial to binary to decimal, problem was trivial.
