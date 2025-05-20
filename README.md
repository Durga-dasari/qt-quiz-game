# qt-quiz-game
This is a lightweight Quiz Game Application built using **Qt C++ and QML**. The game reads questions from a JSON file, displays them through a dynamic QML interface, and manages quiz logic with a custom `QAbstractListModel` in the backend.

## 🚀 Features

- Loads quiz data from a JSON file
- Displays one question at a time with multiple-choice options
- Highlights correct and incorrect answers
- Allows moving to the next question
- Clean separation of UI (QML) and logic (C++)

## 📁 JSON Format

Example structure for `Quiz.json`:

```json
{
  "quiz": [
    {
      "question": "What is the capital of France?",
      "options": ["London", "Berlin", "Paris", "Rome"],
      "answer": "Paris"
    }
  ]
}

## 🧠 Architecture
C++ Backend:
Parses JSON data

Manages quiz state using QAbstractListModel

Exposes data to QML via Qmlsignalshandler singleton

QML Frontend:
Displays questions and options using ListView

Handles user selection and shows result feedback

🔌 Integration
cpp
Copy
Edit
qmlRegisterType<Qmlsignalshandler>("qmlsignalshandler", 1, 0, "Qmlsignalshandler");
This allows QML to access and interact with the C++ backend.

📈 Future Improvements
Add timer and score tracking

Shuffle questions randomly

Add quiz categories and difficulty levels

Store user scores and progress in a file

📄 How to Run
Clone this repo

Place Quiz.json in the correct file path

Open the project in Qt Creator

Build and run the application

🛠 Tools Used
Qt 5/6 (C++ & QML)

QAbstractListModel

JSON Parsing

Feel free to fork, modify, and contribute to the project! 🤝

vbnet
Copy
Edit

Let me know if you’d like a logo, demo GIF, or badges added to the README as well.







