# Guessing-Game-

import random

print("-------------------------------")
print("  M&M Guessing Game!       ")
print("-------------------------------")

print("Guess the number of m&m and you get lunch on the house")
print()

mm_count = random.randint(1, 100)
attempts_limit = 5
attempts = 0

while attempts < attempts_limit:
    guess_text = input("How many m&m are in the jar ")
    guess = int(guess_text)
    attempts += 1

    if mm_count == guess:
        print(f"You got it. It was {guess}.")
        break
    elif guess < mm_count:
        print("Sorry , that too LOW")
    else:
        print("That way too HIGH")

print("Bye")
