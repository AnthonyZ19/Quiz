# Quiz
#Just a simple quiz with Python that includes scoring
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 0]
print('Wanna play a game?')
answer0 = input()
answer1 = answer0.split()
for a in answer1:
  if a in numbers:
    print("no numbers")
    quit()
  elif answer0.lower() == "no":
    print("Ok, then")
    quit()
  elif answer0.lower() == "yes":
    print("Lets get started then")
  elif answer0.lower() != "yes" or "no":
      print("Next time type yes or no")
      quit()
score = 0
print("1. Part of the brain that helps remember new memories is the")
answer1 = input()
if answer1.lower() == "hippocampus":
    print("Correct!, Next Question")
    score += 1
else:
    print("Wrong, Try Again")
    answer1 = input()
    score -= 0.5
while answer1.lower() != "hippocampus":
    print("Wrong, Try Again")
    answer1 = input()
print("2.	Part of the brain that controls hunger and thirst?")
answer2 = input()
if answer2.lower() == "hypothalamus":
    print("Correct!, Next Question")
    score += 1
else:
    print("Wrong, Try Again")
    answer2 = input()
    score -= 0.5
while answer2.lower() != "hypothalamus":
    print("Wrong, Try Again")
    answer2 = input()
print("3.	Which Lobe of the brain allows perception of different textures in what we feel?")
answer3 = input()
if answer3.lower() == "parietal lobe":
    print("Correct!, Next Question")
    score += 1
else:
    print("Wrong, Try Again")
    answer3 = input()
    score -= 0.5
while answer3.lower() != "parietal lobe":
    print("Wrong, Try Again")
    answer3 = input()
print("Well thats it for now")
print("How did you do?")

print("Score: " + str(score))
print("You get one point if you get it right, lose 0.5 if you get it wrong")
