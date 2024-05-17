# my_python_codes

## Coin Toss

```py
import random


print('Welcome to the Coin Toss game!')
print('Guess the result!')


correct_guesses = 0
total_guesses = 0


while True:
  guess = input('\nEnter "heads" or "tails" or "quit" to stop the game -> ')
  if guess == 'quit':
      print("You decided to quit.")
      break
  if guess != 'heads' and guess != 'tails':
      print("Invalid input. Please enter 'heads', 'tails' or 'quit'.")
      continue


  coin = random.randint(0, 1)
  if coin == 0:
      random_result = 'heads'
  else:
      random_result = 'tails'


  if guess == random_result:
      print("Congratulations! You guessed correctly.")
      correct_guesses += 1


  else:
      print(f"Sorry, not correct! It was -> {random_result}.")


  total_guesses += 1
print(f"Correct guesses: {correct_guesses}, Total guesses: {total_guesses}")
```

![image](https://github.com/GitaRac/my_python_codes/assets/165934633/f98dcff1-3818-41d5-8fb8-0808ec51d998)





