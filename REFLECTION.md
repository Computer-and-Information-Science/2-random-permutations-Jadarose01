# Assignment 2 Reflection - JADA ROSE

## Approach to the Problem

I approached this assignment by carefully reviewing the descriptions of the three algorithms and identifying the differences in how each generates a random permutation. My first step was to outline the logic of each algorithm in pseudocode before translating it into C++. I then worked on one algorithm at a time, starting with the most straightforward (Algorithm 1), and verified correctness before moving to the next. Once all three algorithms were implemented, I tested them with smaller array sizes to confirm they produced valid permutations before running the larger timing experiments.

## Techniques Used

To solve the problem, I used modular programming techniques by keeping each algorithm in its own function. I also used helper structures such as a boolean *used* array for Algorithm 2 and the Fisher–Yates shuffle for Algorithm 3. For Algorithm 1, I relied on the provided *search* function to ensure uniqueness of values. I made use of loops, conditional checks, and the *randint* utility functions to generate random numbers within the required ranges. I also ran the program multiple times with different command-line arguments to automate timing tests and gather data efficiently.

## Challenges Encountered

One of the main challenges was implementing Algorithm 1 efficiently, since checking for duplicates with a linear search became slow for larger array sizes. This made testing with big inputs take significantly longer compared to the other algorithms. Another challenge was ensuring that Algorithm 3’s shuffle was implemented correctly, since an incorrect shuffle could bias the randomness of the permutation. I overcame these challenges by reviewing the Fisher–Yates algorithm (referencing online resources such as GeeksforGeeks and lecture slides), double-checking index ranges, and verifying that each algorithm generated valid permutations by inspecting smaller test cases before scaling up.

## Conclusions

From this assignment, I learned how different algorithmic approaches to solving the same problem can have dramatically different time complexities and performance outcomes. Algorithm 1 was quadratic in nature and quickly became impractical, Algorithm 2 improved performance with linear time complexity but still required retries on duplicates, and Algorithm 3 was the most efficient and elegant solution, consistently scaling well to very large arrays.
