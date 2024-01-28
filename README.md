# Sudoku
This implementation consists of 2 phases. Phase 1 tell whether consists of designing a multithreaded application that determines whether the solution to a Sudoku puzzle is valid or not. Phase 2 will give the result of an unsolved Sudoku puzzle.

I have made 3 functions, 
The first function is to check the rows of the matrix. It uses 2 for loops to check 
each element of the matrix, the first loop is updating the row number of the 
element and the second is updating the column number of the element. I have 
added an array and it compares each element with the array. If the row values are 
1-9 the check is true and the row is valid. If not, the row is not valid.
The second function is to check the column of the matrix. It uses 2 for loops to 
check each element of the matrix, the first loop is updating the row number of 
the element and the second is updating the column number of the element. I 
have added an array and it compares each element with the array. If the column 
values are 1-9 the check is true and the column is valid. If not, the column is not 
valid.
The third function is to check the 3x3 matrix box of the matrix. It uses 2 for loops 
to check each element of the matrix, the first loop is updating the row number of 
the element (and it only runs for the 3 consecutive rows) and the second is 
updating the column number of the element (and it only runs for the 3 
consecutive columns). I have added an array and it compares each element with 
the array. If the box values are 1-9 the check is true and the box is valid. If not, the 
box is not valid.
We have used joinable threads in this case to implement the SUDOKO SOLVER 
AND VALIDATOR. So the threads work in Parallel which decreases computation 
time and system resources are used more efficiently. All the threads are joined 
with the main driver thread which receives the resources released by each thread 
for further processing. We have used mutex lock in the Solver to avoid the board 
to be read while the change is being updated.
