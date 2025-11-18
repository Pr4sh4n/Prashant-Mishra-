import random

print("🎯 Welcome to the Number Guessing Game!")
print("I'm thinking of a number between 1 and 50.")

# Generating random number
secret_number = random.randint(1, 50)

# Infinite loop until correct guess
while True:
    guess = int(input("Enter your guess: "))

    if guess < secret_number:
        print("Too low! Try again ⬆")
    elif guess > secret_number:
        print("Too high! Try again ⬇")
    else:
        print("🎉 Correct! You guessed the number!")
        break
