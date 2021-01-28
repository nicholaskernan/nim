# nim

My nim game can be played at: https://codepen.io/nicholaskernan/pen/gOpbzxx

The rules of nim are explained there. 

This version is a bit untraditional, in that the number of piles and number of stones in each pile are randomized each time.

However, the basic strategy remains the same. In general, the optimal move will be one that causes the "nim-sum" to be 0. 

Thus, if the stones are mentally grouped into groups of 4, 2 and 1 stone, the winning move will cause the number of each of these groups to be even.
For example, if there are 8 stones in one pile and 5 stones in another, there are 3 groups of 4, 0 groups of 2 and 1 group of 1. To even out the groups, remove 3 stones from the 8 stone pile, such that both piles have 5 stones. Thus, there will be 2 groups of 4 and 2 groups of 1 - even numbers. 

For a more thorough explanation: https://www.archimedes-lab.org/How_to_Solve/Win_at_Nim.html

It is always possible to even out the groups if they are not currently even, and never possible to keep it even if it already is. Thus, a board position with a nim-sum already equal to 0 is a losing position, because you cannot set it equal to 0. 

The nim-sum rules do not always apply to simple board states. For example, if it is your turn when there is 1 stone in each of three piles, it is a losing position even though you can set the nim-sum equal to 0. 
