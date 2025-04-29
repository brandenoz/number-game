<p align="center">
 <img src="https://github.com/user-attachments/assets/784c1a3e-f470-4234-ac8f-d98ff29eff9c" alt="Python Logo" width=20%/>
 </p>

 <h1>Number Guessing Game</h1>
 The Python code will pick a number from 1-100. It will be random each time. It will tell you one of three things: you guessed correctly, you guessed too high, or you guessed too low.  
 
 <h2>Code</h2>
 
```python
import random
import time

print("Hi! Welcome to the guessing game. I am going to pick a number between 1 and 100.")
time.sleep(3)
print("Picking a number...")
time.sleep(2)
guess = int(input("What is your guess?: "))
correct_number = random.randint(1,100)
guess_count = 1

while guess != correct_number:
  time.sleep(1)
  guess_count += 1
  if guess < correct_number: 
    guess = int(input("Wrong. You need to guess higher. what is your guess?: "))
  else: guess = int(input("Wrong. You need to guess lower. what is your guess?: "))

print(f"Congrats! The right answer was {correct_number}. It took you {guess_count} guesses.")
```
 
 <h2>Example Gameplay</h2>

- Initially, you will be prompted to guess a number. There is time built in for the program while picking a number to appear that it is taking a second to think. This humanizes the game element just a bit. 

![Python_1st](https://github.com/user-attachments/assets/8742d90d-fbf1-4b2e-ba5b-3314fb6c64a9)

- After a few guesses you should be able to get it correct using the hints. 

![Correct_Guess](https://github.com/user-attachments/assets/03ab12c3-5902-4aca-9fc6-35515029aaf5)

- To see other projects click here: https://github.com/brandenoz. 
