This is our answer to Question 2 of the NBA Basketball Analytics Track.

In this zip you will find:
Question_2.ipynb: Python Notebook
Question_2.pdf: PDF of python code
Question_2.py: Python code
elimination_results.csv: results

High Level Overview of Solution
We solved question 2 using Python. The approach broke down the data into different days, all containing a number of games, as well as relevant information about the teams and standings at that point in time. To begin, we uploaded all the data and calculated league standings throughout the season. At the end, we determined which 8 teams from each conference made the playoffs. The next part was to determine the date the remaining 14 teams were eliminated from playoff contention. Our strategy was to work backwards, starting at the end of the last game of the season. We then went backwards a day at a time, trying to find the first day when a team was no longer eliminated from the playoffs. Once this day was found, the following day is consequently when they were first eliminated. We did this by simulating the best case scenario for a team for each day until a path to the playoffs for that team was found.
