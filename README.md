

questions = ("Which of the following galaxies is closest to the Milky Way?",
             "What is the primary gas in the atmosphere of Jupiter?",
             "What is the approximate age of the universe?",
             "Which of the following planets has the longest day (rotation period) in our solar system?",
             "What is the largest moon of Saturn?",
             )
options =(("a) Andromeda","b) Triangulum","c) Whirlpool","d) Messier 87"),
          ("a) Nitrogen","b) Oxygen","c) Hydrogen","d) Helium"),
          ("a) 5 billion years ","b) 10 billion years","c) 13.8 billion years","d) 20 billion years"),
          ("a) Venus","b) Mars","c) Jupiter","d) Neptune"),
          ("a) Titan","b) Enceladus","c) Rhea","d) Mimas"))
answers =("a","c","c","a","a")
guesses =[]
score = 0
question_num =0
for question in questions:
    print("---------------")
    print(question)
    for option in options[question_num]:
        print(option)
    guess =input("Enter(a,b,c,d):").lower()
    guesses.append(guess)
    if guess ==answers[question_num]:
        score += 1
        print("CORRECT!!")
    else:
        print("INCORRECT!!")
        print(f"{answers[question_num]} is the correct answer..")
    question_num +=1

    print("---------------")
    print("    RESULTS    ")
    print("---------------")

    print("answers:",end="")
    for answer in answers:
        print(answer,end="")
    print()

    print("guesses:", end="")
    for guess in guesses:
        print(guess, end="")
    print()

