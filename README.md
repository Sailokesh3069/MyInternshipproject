# MyInternshipproject

import random

class QuizGame:
    def __init__(self):
        self.questions = [
            {"question": "What is the capital of France?",
             "options": ["A. Paris", "B. London", "C. Berlin"],
             "correct_answer": "A"},
            {"question": "Which programming language is known for its readability?",
             "options": ["A. Python", "B. Java", "C. C++"],
             "correct_answer": "A"},
            {"question": "What is the largest mammal?",
             "options": ["A. Elephant", "B. Blue Whale", "C. Giraffe"],
             "correct_answer": "B"}
        ]
        self.score = 0

    def display_question(self, q):
        print(q["question"])
        for option in q["options"]:
            print(option)
        user_answer = input("Your answer (Enter A, B, or C): ").upper()
        return user_answer

    def check_answer(self, user_answer, correct_answer):
        if user_answer == correct_answer:
            print("Correct!\n")
            self.score += 1
        else:
            print(f"Incorrect. The correct answer is {correct_answer}.\n")

    def run_quiz(self):
        print("Welcome to the Basic Quiz Game!\n")
        for question in self.questions:
            user_answer = self.display_question(question)
            self.check_answer(user_answer, question["correct_answer"])

        print(f"Quiz completed. Your final score is: {self.score}/{len(self.questions)}")

if __name__ == "__main__":
    quiz = QuizGame()
    quiz.run_quiz()




https://github.com/Sailokesh3069/MyInternshipproject/assets/162870856/369fb459-7c0a-4a2a-90cc-b81aaea8f251


https://github.com/Sailokesh3069/MyInternshipproject/assets/162870856/da60c682-8727-4e33-83f7-698971dc4bb2



