## Exercise 4: Primitive Quiz - 30 Marks

In this exercise, you'll create a simple program that asks the user a question, evaluates their answer, and provides feedback.

### Steps:
1. Write a program that asks the user "What is the capital of France?" and waits for their response.
2. If the user's answer is correct (i.e., "Paris"), the program should print a message saying the answer is correct.
3. If the answer is incorrect, the program should print a message saying the answer is wrong.

### Advanced Requirements:
Ignore Capitalization: Modify your program to accept answers regardless of the capitalization (e.g., "paris", "Paris", and "PaRis" should all be considered correct).
Multiple Questions: Extend the program into a quiz that asks for the capitals of 10 European countries. Provide feedback for each question.
def quiz():
questions = {"France": "Paris","Germany": "Berlin","Italy": "Rome","Spain": "Madrid","Portugal": "Lisbon", "Netherlands": "Amsterdam","Belgium": "Brussels","Switzerland": "Bern", "Austria": "Vienna","Poland": "Warsaw"}
       print("Welcome to the European Capitals Quiz!")
 for country, capital in questions.items():
        answer = input(f"What is the capital of {country}?)
  if answer.lower() == capital.lower():
            print("Correct!")
        else:
            print(f" Wrong. The capital of {country} is {capital}.")
  if __name__ == "__main__":
        quiz()

