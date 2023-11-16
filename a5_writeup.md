# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. How do the performance and efficiency of the Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms compare when solving Sudoku puzzles? In what scenarios might one approach be preferable over the other?
Both DFS and BFS were equal in terms of efficiency for an easier board while DFS was more efficient on a more complex board. DFS would be more preferable if the solution would be within the first couple iterations into a branch rather than towards the end where it won't have to do every possible combination to get a solution. Meanwhile BFS would benefit if the solution didn't require as many inputs and was shallow in the ability to find a solution quickly from the surface of the board it is solving for.



2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?
DFS would be more effective on solving a board that has more choices while BFS would be better on a less complex board that can find a solution relatively quickly due to an answer being more obvious to choose from. An alternative data structure could be pushing a board within the middle of the list in which an algorithm could focus on doing half the board through a BFS kind of way to reduce the number of inputs. If a solution isn't found then it would move on to the other half of the board.


3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?
I think that the Sudoku solver could be adapted to a grid based logic game just through using BFS or DFS. A game like Minesweeper would seem to probably benefit from BFS as the board doesn't necessarily seem complex so finding a solution wouldn't seem too deep. In a real world application, it might be beneficial to think about using a DFS type of method in solving a problem. Most people subconsciously (myself included) probably do BFS and using DFS could be advantageous for certain problems as not everything can be solved efficiently through a single method.

