# Compiler Design: Top Down Parser

## ✅ Features 

- [X] Provide Rules and Input to check if the input string is valid as per the rules

### 💡 Note:
- The Rules should not have left recursion.


**Example:**

```
E -> E+T | E-T | T
T -> T*F | T/F | F
F -> 0|1|2|3|4|5|6|7|8|9
contains Left Recursion

```

_After eliminating Left Recursion:_

```
E -> TA
A -> +TA | -TA | e
T -> FB
B -> *FB | /FB | e
F -> 0|1|2|3|4|5|6|7|8|9
There are total 18 rules and starting Non Terminal symbol is E.

The Input should end with '$' example: 5+6/7*8-9+8$
```

### 💡 Note:
👉 See the Example.txt file for more understanding of using the parser


