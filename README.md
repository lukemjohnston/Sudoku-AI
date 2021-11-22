# Sudoku-AI

This was an assignment for my AI class. I really enjoyed working on this one!


Sudoku can be viewed as a CSP.  

The variables are the individual cells, numbered 0 to 80, based on the location on the board. A cell 
located in row a (can be 0 to 8) and column b (can be 0 to 8), will have index 9*a+b. 

The constrains are converted to binary constraints and given by the constraints graph, represented by a 
boolean matrix C[81][81], where C[x][y]=true if and only if cells x and y must be different (i.e., x and y 
are in the same row, same column, or same 3x3 subgrid). 

The domain for each of the variables are the numbers 1 to 9 and represented by an array of vectors,  
vector<int> domain[81].  Each individual Sudoku puzzle comes with a predefined assignment of values 
for particular cells (unary constraints).  We reflect these unary constraints immediately on the domain.  
For example, if cell (variable) indexed by 70 is defined by the puzzle to be 4, then domain[70]={4} 
(instead of {1,2,3,4,5,6,7,8,9}). 
  
An assignment is the assigning of a specific value to each cell (variable) and is represented by a vector of 
integers,  vector<int> assignment.
