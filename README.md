# Yvonne's Leetcode-Problem Solving
Here is my email : <ywuyvonne@gmail.com>\
Weclome to [Yvonne's Leetcode's Link](leetcode-cn.com/u/yvonnewu/).     
My NoteBook for the [Basic Knowledge](https://github.com/Luchanaaaaa/LeetCode/blob/main/baseKnowledge.md)

## Online Assement 
1. [Job scheduling](https://github.com/Luchanaaaaa/LeetCode/issues/2)
## Array
[56. Merge Intervals](https://github.com/Luchanaaaaa/LeetCode/issues/4).       
[704. Binary Search](https://github.com/Luchanaaaaa/LeetCode/issues/5)
 
## Backtracking
### What is Backtracking?
Backtracking is a general algorithm for finding all (or some) solutions to a problem incrementally by trying out potential solutions, and abandoning a potential solution as soon as it proves to be unfeasible. It is typically used for problems that can be broken down into smaller subproblems, where the problem is to find a solution among all possible combinations of the subproblems.  

Backtracking is commonly used to solve several types of problems, including:

1. Combination problems: finding all possible combinations of *N* elements, subject to certain rules   
[77. Combinations](https://github.com/Luchanaaaaa/LeetCode/issues/3)

2. Cutting problems: finding all possible ways of cutting a string, subject to certain rules.  
3. Subset problems: finding all possible subsets of N elements that meet certain conditions
4. Permutation problems: finding all possible permutations of N elements, subject to certain rules
5. Chessboard problems: solving problems like the N-Queens problem, where the goal is to place N queens on a chessboard so that no two queens attack each other.

These problems can all be solved using backtracking by incrementally constructing a solution, and checking the feasibility of each partial solution before proceeding to the next step.   

### Three Step to think about *Backtracking*.  
1.  *Return value* and *Argument* of the Backtraking Funciton.     
The Return value usually is void.   
```java
Public void backtracking(){
}
``` 
2. Backtracking function termination condition. 
```java
Public void backtracking(){
  if( Termination condition ){
      Store the Result
      return;
  }
``` 
3. Traversal process of backtracking search.   
```java
Public void backtracking(){
  if( Termination condition ){
      Store the Result
      return;
  }
  for ( The same layer in the tree) {
      Process the node;
      Backtracking (path) //Recursion
      backtracking
      
     
  }
}  
``` 

 
## Dynamic Programming
[5. Longest Palindromic Substring](https://github.com/Luchanaaaaa/LeetCode/issues/6)



## Stack
[20. Valid Parentheses]([./Stack/stackQuestion.md](https://github.com/Luchanaaaaa/LeetCode/issues/1))


