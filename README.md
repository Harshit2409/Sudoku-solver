# Sudoku-solver
### Sudoku puzzle generator &amp; solver
This is a simple Sudoku solver in which a random sudoku puzzle is generated & solved by the computer. It is written using JavaScript, HTML & CSS.

![Image of web app](https://github.com/Harshit2409/Sudoku-solver/blob/master/images/Screenshot%202020-10-12%20161840.png)
## **Implementation**
#### Sudoku generation:
Sudoku is generated using a API

API:-https://sugoku.herokuapp.com/board?difficulty=easy

GITHUB link: - https://github.com/berto/sugoku

HTML & CSS is used for creating and styling of the web page.
JavaScript is the main component which solve the randomly generated sudoku puzzle. The Algorithm uses recursion and backtracking for finding the most optimal solution for the puzzle

## **Pseudocode: -**
```
bool Solve(configuration conf)
{
   if (no more choices) // BASE CASE  
      return (conf 1 goal state);
for (all available choices) {
    try one choice c;    
    // solve from here, if works out, you're done
    if (Solve(conf with choice c made)) return true;
    unmake choice c:
    }
return false: // tried all choices, no solution
}
```
