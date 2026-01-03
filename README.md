# A-simple-survey-2
This is a simply survey #2. Here, I added 3 attempts  for the user to guess their age in 3 years.


q = input("Hi! What's your name?")
m = int(input("How old are you?"))

correct_number = m + 3

print("Please, guess your age in 3 years!")

for attempt in range(1, 4):
    guess = int(input(f"Attempt {attempt}: Your guess? "))
    
    if guess == correct_number:
        if attempt == 1:
            print("Wow, genius!")
        else:
            print("Good job!")
        break 
    else:
        print("Try again!")
else:
    print(f"Too bad! The number was {correct_number}")
