# Alex                                                 ALEKSANDAR LAZAREVIC


ALGORITHM FOR SOLVING THE SUBVARIANT OF THE “ THE SUM OF A SUBSET 

PROBLEM ” IN POLINOMYAL TIME.





                                                         1. Introduction


The problem that the presented algorithm solves is also known as the "Two Towers Problem".The task that the algorithm should perform is to divide the set of integers into two subsets whose sums of members are equal. As half of the total sum of the whole set is only one of many that exist in it, we can say that this problem is just another variant of the "Subset sum problem". When it comes to sets with a small number of members, checking whether the task can be done and what the exact solution is, is not a special problem. But with a set of only 100 members, the number of combinations grows to 1,267,650,600,228,229,401,496,703,205,376 and solving every possibility (Brut-force) loses all meaning because the time required to check is enormous.


                                        2. The principle of operation of the algorithm


   The first thing to note is that for the algorithm to work properly, the members of the set must be entered in order from smallest to largest.
   The algorithm first calculates the sum of all members of the set "a" (N) and then half of that sum (S). After that, it checks whether there is a member of the set "a", whose value is equal to S.
Depending on whether S is less than or greater than 0, a certain piece of code is executed.
 Then it forms an imaginary set "b" of the members of the set "a" by adding the members starting from the largest member of the set "a" by adding them until the value of their sum (M) exceeds S. We now have an imaginary set "b" in which the sum of all terms is close to the value of S.
The algorithm prints the members of set "b".
At this point, the variable Q is introduced, which represents the addition values of all members of the set "b" in order from largest to smallest. The algorithm checks whether Q is equal to S.
The algorithm checks whether Q is increased by the value of the set member of set “a”is equal to S. The algorithm checks whether Q is increased by the value of the set member of set “a” reduced by the value of set member "b" and increased by another member of the set "a" is equal to S.



                                                                  

In case any of the assumed equations is correct, the algorithm prints the required values on the screen.
In case when S  is less then 0 , there is an additional line of code  “ if (a[i] < 0)”.


