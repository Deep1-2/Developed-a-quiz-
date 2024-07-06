# Developed-a-quiz-
#Python Quiz Application
questions = {
    "What is the capital of France?": "Paris",
    "Which planet is known as the Red Planet?": "Mars",
    "What is the capital of India?" : "Delhi",
    "Who is the father of the computer?" : "Charles babbage",
    "Who developed Python programming Language?" : "Guido van Rossum",
    "Python is case sensitive language ?" : "Yes",
}
def main():
    score = 0
    for question, correct_answer in questions.items():
        user_answer = input(f"{question} ")
        if user_answer.lower() == correct_answer.lower():
            print("Correct!")
            score += 1
        else:
            print(f"Sorry, the correct answer was {correct_answer}.")
    print(f"Your final score: {score}/{len(questions)}")
    if score == len(questions):
        print("Great job! You aced the quiz.")
    else:
        print("Keep practicing!")

if __name__ == "__main__":
    main()
