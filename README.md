# 538_older_than_L
Jupyter Julia notebook to solve 538 riddler puzzle.

https://fivethirtyeight.com/features/dont-trust-anyone-older-than-l/

Program first defines the truth-telling and lying versions of each islander as a function that returns a boolean value.
It then goes into a loop that cycles through every possible combination of ages between 16 and 22 (the lowest and highest
comparisons made) for each islander, as well as for the threshold at which they begin lying.
The loop also checks these ages against every possible combination of the truth-telling/lying functions.
The loop will print the ages when the following conditions are met...
- all of the functions show true given the age inputs (they work, either as truth-telling or lying, for the given ages)
- an array showing true/false whether a given islander is older than L (aka they are lying) matches an array showing 
  the result of the truth-telling statement. This checks that each islander lying matches the islanders that should be lying
  according to their age.
