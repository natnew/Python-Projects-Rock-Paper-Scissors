# Python Projects Rock Paper Scissors 🐍
Python Script <br>
This repo contains python code that generates a rock, paper, scissors game. <br>
Run the code.

Python
```python
import random

def play():
    user = input("What's your choice? 'r' for rock, 'p' for paper, 's' for scissors")
    computer = random.choice(['r', 'p', 's'])

    if user == computer:
        return 'It is a tie'

    if is_win(user, computer):
        return 'You won!'

    return 'You lost!'

   
def is_win(player, opponent):
    if (player == 'r' and opponent == 's') or (player == 's' and opponent == 'p') or (player == 'p' and opponent == 'r'):
        return True

print(play())
```

Output
```s
You Won!
```
