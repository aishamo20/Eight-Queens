# ♛ Eight Queens

*Placing 8 queens on a chessboard so that none can attack each other.*

## The puzzle

A queen in chess can attack along its row, its column and both diagonals.
The challenge is to place 8 queens on a standard 8×8 board so that no two
queens threaten each other. There are 92 possible solutions.

## How it works

The program places one queen per row, starting from the top. For each row,
it tries each column and checks whether that square is safe from all the
queens already placed. If it is, it moves on to the next row. If no square
in a row is safe, it goes back to the previous row and moves that queen to
the next option. This technique is called **backtracking**.

## Example output

```
Q . . . . . . .
. . . . Q . . .
. . . . . . . Q
. . . . . Q . .
. . Q . . . . .
. . . . . . Q .
. Q . . . . . .
. . . Q . . . .
```

## What I learned

- How recursion and backtracking can solve search problems efficiently
- Breaking a puzzle into small checks (rows, columns, diagonals)
- Building a project step by step and testing as I go
