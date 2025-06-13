# Quiz-game
# 10-question quiz game in Python

def run_quiz():
    questions = [
        {
            "question": "What is the capital of France?",
            "options": ["A. Berlin", "B. Paris", "C. Madrid", "D. Rome"],
            "answer": "B"
        },
        {
            "question": "Which planet is known as the Red Planet?",
            "options": ["A. Venus", "B. Jupiter", "C. Mars", "D. Saturn"],
            "answer": "C"
        },
        {
            "question": "Who wrote 'Romeo and Juliet'?",
            "options": ["A. Charles Dickens", "B. Mark Twain", "C. William Shakespeare", "D. Jane Austen"],
            "answer": "C"
        },
        {
            "question": "What is the largest mammal in the world?",
            "options": ["A. Elephant", "B. Blue Whale", "C. Giraffe", "D. Hippopotamus"],
            "answer": "B"
        },
        {
            "question": "Which element has the chemical symbol O?",
            "options": ["A. Oxygen", "B. Gold", "C. Iron", "D. Osmium"],
            "answer": "A"
        },
        {
            "question": "Which language is used for web apps?",
            "options": ["A. Python", "B. Java", "C. JavaScript", "D. C++"],
            "answer": "C"
        },
        {
            "question": "Who painted the Mona Lisa?",
            "options": ["A. Pablo Picasso", "B. Vincent Van Gogh", "C. Leonardo da Vinci", "D. Michelangelo"],
            "answer": "C"
        },
        {
            "question": "How many continents are there on Earth?",
            "options": ["A. 5", "B. 6", "C. 7", "D. 8"],
            "answer": "C"
        },
        {
            "question": "Which is the smallest prime number?",
            "options": ["A. 0", "B. 1", "C. 2", "D. 3"],
            "answer": "C"
        },
        {
            "question": "What gas do plants absorb from the atmosphere?",
            "options": ["A. Oxygen", "B. Nitrogen", "C. Carbon Dioxide", "D. Hydrogen"],
            "answer": "C"
        }
    ]

    score = 0

    for i, q in enumerate(questions, 1):
        print(f"\nQuestion {i}: {q['question']}")
        for option in q["options"]:
            print(option)
        user_answer = input("Your answer (A/B/C/D): ").strip().upper()

        if user_answer == q["answer"]:
            print("✅ Correct!")
            score += 1
        else:
            print(f"❌ Wrong! The correct answer is {q['answer']}.")

    print(f"\n🎉 Quiz Over! You scored {score} out of {len(questions)}.")

if __name__ == "__main__":
    run_quiz()
