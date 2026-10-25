Crossword Puzzle Solver

📌 Project Overview

This project solves the **Crossword Puzzle** problem using the **Backtracking Algorithm** in Java. The program fills a 10 × 10 crossword grid with a given list of words by placing them horizontally or vertically while satisfying the puzzle's constraints.

🎯 Problem Statement

A 10 × 10 crossword grid is provided along with a list of words separated by semicolons. The cells marked with `-` must be filled with the given words.

* `+` represents blocked cells.
* `-` represents empty cells that need to be filled.
* Words must fit into the available horizontal or vertical slots.
* Letters at intersecting positions must match correctly.

🛠️ Technologies Used

* **Programming Language:** Java
* **Algorithm:** Backtracking
* **Data Structures:** 2D Character Array, String Array, Boolean Array, ArrayList
* **Platform:** HackerRank

⚙️ Algorithm Used: Backtracking

Backtracking is an algorithmic technique that explores possible solutions and reverses a choice when it leads to an incorrect result.

Steps Involved

1. **Read the Crossword Grid:** Store the 10 × 10 grid in a two-dimensional character array.
2. **Read the Words:** Split the input string using a semicolon (`;`) and store the words in an array.
3. **Track Used Words:** Use a Boolean array to identify words that have already been placed.
4. **Find Valid Slots:** Search for horizontal and vertical slots where words can begin.
5. **Check Word Placement:** Verify that the word length matches the slot and that existing letters do not conflict.
6. **Place the Word:** Insert the word into the grid and save the previous cell values.
7. **Backtrack:** If a placement does not lead to a solution, restore the previous grid values and try another word.
8. **Return the Solution:** Convert the completed grid into a list of strings.

💻 Sample Input

```text
+-++++++++
+-++++++++
+-++++++++
+-----++++
+-+++-++++
+-+++-++++
+++++-++++
++------++
+++++-++++
+++++-++++
LONDON;DELHI;ICELAND;ANKARA
```

✅ Sample Output

```text
+L++++++++
+O++++++++
+N++++++++
+DELHI++++
+O+++C++++
+N+++E++++
+++++L++++
++ANKARA++
+++++N++++
+++++D++++
```

🧠 Key Concepts Learned

* Understanding and implementing the backtracking algorithm.
* Using recursion to explore possible solutions.
* Finding horizontal and vertical word slots.
* Validating word placements against existing letters.
* Restoring the grid when a placement fails.
* Applying algorithmic problem-solving to a constraint-based puzzle.

⏱️ Time Complexity

The backtracking algorithm may explore multiple possible word placements. In the worst case, the search can grow exponentially with the number of words. The actual execution time depends on the crossword grid and the number of possible placements.

🔗 References

* **HackerRank Problem:** [Crossword Puzzle](https://www.hackerrank.com/challenges/crossword-puzzle/problem)
* **GitHub Repository:** [DAA_ASSIGNMENT – Crossword Puzzle](https://github.com/Puji-6/DAA_ASSIGNMENT/blob/main/Crossword%20Puzzle)


