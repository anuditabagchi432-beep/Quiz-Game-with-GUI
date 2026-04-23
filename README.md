# Quiz-Game-with-GUI

quiz game with gui (GRAPHICAL USER INTERFACE) in python

def play_quiz():
    questions = [
        {"q": "What is 2 + 2?", "a": "4"},
        {"q": "What is the capital of France?", "a": "Paris"},
        {"q": "Which language is used for AI?", "a": "Python"},
        {"q": "What is the capital of Astralia?", "a": "Sydney"},
        {"q": "What is 22*9?", "a": "198"},
        {"q": "Which is the most spoken language in India?", "a": "Hindi"}
    ]
    
    score = 0
    print("--- Welcome to the Text Quiz ---")
    
    for item in questions:
        answer = input(f"{item['q']} ")
        if answer.lower() == item['a'].lower():
            print("Correct!")
            score += 1
        else:
            print(f"Wrong! The answer was {item['a']}.")
            
    print(f"\nGame Over! Final Score: {score}/{len(questions)}")

if __name__ == "__main__":
    play_quiz()
