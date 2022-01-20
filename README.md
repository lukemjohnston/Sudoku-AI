# Sudoku-AI

This was an assignment for my AI class. I really enjoyed working on this one!


Sudoku can be viewed as a CSP.  

Assigment description:
  
  "The variables are the individual cells, numbered 0 to 80, based on the location on the board. A cell 
  located in row a (can be 0 to 8) and column b (can be 0 to 8), will have index 9*a+b. The constrains are converted to binary constraints and given by the constraints graph, represented by a boolean matrix C[81][81], where C[x][y]=true if and only if cells x and y must be different (i.e., x and y are in the same row, same column, or same 3x3 subgrid). The domain for each of the variables are the numbers 1 to 9 and represented by an array of vectors, vector<int> domain[81].  Each individual Sudoku puzzle comes with a predefined assignment of values for particular cells (unary constraints).  We reflect these unary constraints immediately on the domain.  For example, if cell (variable) indexed by 70 is defined by the puzzle to be 4, then domain[70]={4} (instead of {1,2,3,4,5,6,7,8,9}). An assignment is the assigning of a specific value to each cell (variable) and is represented by a vector of integers,  vector<int> assignment."
  
  
Here is how the sudoku puzzle is represnted and then simplified to only the possible actions.
![AI_puzzle_AC3](https://user-images.githubusercontent.com/72853815/150280479-06733082-95a8-4a24-8125-7d8d2307a194.PNG)
![AI_CSP](https://user-images.githubusercontent.com/72853815/150280424-5035e5de-dc0d-4e3e-918b-73445718e557.PNG)
![AI_CSP_AC3](https://user-images.githubusercontent.com/72853815/150280433-0ee00650-fc52-4baf-b244-acb2ab089f2e.PNG)

    
  
Here are some examples of it solving puzzles:
  
ex #1
  
![AI_puzzle1](https://user-images.githubusercontent.com/72853815/150278616-0e042ee2-1ee9-4ad9-9a2e-e9d954719cd5.PNG)
![AI_solved1](https://user-images.githubusercontent.com/72853815/150278622-0bf8ffa1-589a-4467-8b54-db4d98dc9859.PNG)
  
 
ex #2 
  
![AI_puzzle2](https://user-images.githubusercontent.com/72853815/150279052-2727d0ad-069a-42c6-8ae9-a06de03a74d7.PNG)
![AI_solved2](https://user-images.githubusercontent.com/72853815/150278919-fd5d7865-fc49-4852-ab7c-957ed21d7ab7.PNG)


  
