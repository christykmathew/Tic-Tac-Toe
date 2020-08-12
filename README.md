<a href="https://www.python.org/downloads/release/python-383/"><img src="https://img.shields.io/badge/Python-v3.8-blue"></a>

# Tic-Tac-Toe
A simple python program for Tic-Tac-Toe. <i>Random</i> package is used by the program for computer move

<h2>Working</h2>
<i>check</i> function is used to check whether three symbol marks are present in horizontal, vertical or diagonal direction.<br>
During computer move program checks if comp wins if the symbol placed on a particular postion

```python
.
.
for i in (free):
        row,col = i
        temp = deepcopy(board)
        temp[row][col] = player['comp']
        if(check(temp, player) != 0):
            index = free.index([row,col])
            del free[index]
            return row,col
.
.
```
If not found, then checks if human wins if the symbol placed on a particular postion

```python
.
.
for i in (free):
        row,col = i
        temp = deepcopy(board)
        temp[row][col] = player['hooman']
        if(check(temp, player) != 0):
            index = free.index([row,col])
            del free[index]
            return row,col
.
.
```
Else it gives a random move from the free positons available.

```python
.
.
row,col = r.choice(free)
  index = free.index([row,col])
  del free[index]
  return row,col
.
.
```
