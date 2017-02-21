# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: I guess the question should be 'How does Naked twin method make constraint propagation works faster?' (Sorry. I'm not a native speaker.)
As this techniques helps us eliminate possiblities of the common peer(s) that has either or both posible digit of the Naked twins,
we will have less time of running the depth-first-search for those possibility we've eliminated. It makes our program runs faster.

# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: For a diagonal Sudoku compared to a normal one, we have to consider an additinal set of diagonal peer if a box is in ['A1','B2','C3',...,'I9'] or ['A9','B8','C7',...,'I1'].
(Consider both diagonal peers if the box is 'E5')
Luckily, the provided codes has already had a good way to create the unit dictionary and the peer dictionary from the unitlist list.
What I needed to do was adding 2 more list of diagonal unit into the provided unitlist list. Diagonal peers will be added to the peer dictionary. Hooray!

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project. 
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solutions.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in solution.py

### Data

The data consists of a text file of diagonal sudokus for you to solve.