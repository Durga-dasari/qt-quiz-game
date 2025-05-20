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

## 🏗 Architecture
The project separates logic and UI using a model-view architecture.












