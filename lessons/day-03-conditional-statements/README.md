# Day 3 — Conditional Statements: `if`, `elif`, `else`

⏱️ **Duration:** 120 minutes  ·  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/homaira-mohammadi/python-for-beginners/blob/main/lessons/day-03-conditional-statements/lesson.ipynb)

Students teach Python to make decisions: comparison operators, `if`, `else`, `elif`, logical operators, and a first game.

## 🎯 Learning objectives

- Write conditions with `== != > < >= <=`
- Use `if`, `else` and `elif`
- Combine conditions with `and`, `or`, `not`
- Build interactive programs and a simple game

## 📁 Files in this lesson

| File | What it is |
|---|---|
| [`slides/Day-03-Conditional-Statements.pdf`](slides/Day-03-Conditional-Statements.pdf) | Slides (view on GitHub) |
| [`lesson.ipynb`](lesson.ipynb) | 📘 The full lesson — explanations + code you can run |
| [`exercises.ipynb`](exercises.ipynb) | ✏️ Exercises for students (empty code cells) |
| [`solutions.ipynb`](solutions.ipynb) | ✅ Example solutions with output |

## 🧠 Key concepts

| Concept | Explanation |
|---|---|
| Condition | A yes/no question that Python answers with `True` or `False`: `age >= 18` |
| `=` vs `==` | `=` stores a value, `==` compares two values |
| `if` | Runs the indented block only when the condition is True. Needs a colon `:` and 4-space indentation. |
| `else` | Runs when the `if` is False. It has no condition. |
| `elif` | Checks another condition. Python checks from top to bottom and stops at the first True — order matters! |
| `and` / `or` / `not` | Both must be True / at least one is True / flip True ↔ False |

## 🧑‍🏫 Suggested class plan

| Time | Activity |
|---|---|
| 15 min | Speed round warm-up (review of Days 1–2) |
| 10 min | *Why do programs need decisions?* |
| 25 min | Comparison operators, `if`, prediction challenge, `if` with input, common mistakes |
| 20 min | `else` + Pass/Fail challenge + even/odd |
| 25 min | `elif` + grade examples + why order matters |
| 15 min | Logical operators and nested `if` |
| 10 min | Game: Guess the Number / Rock, Paper, Scissors |

## ✨ Added in this improved version

Compared to the original slides, the notebook adds:

- Logical operators `and`, `or`, `not` (listed in the slide goals, but not covered)
- A game: *Guess the Number* and *Rock, Paper, Scissors* (promised in the slide goals)
- Mistakes: missing colon, missing indentation, `=` instead of `==`
- *Why order matters* in `elif` chains, nested `if`
- Flowcharts that render on GitHub
- 11 exercises incl. a *BMI checker* mini project

## 📌 Note

**Slide fix needed:** on slide 7 of the PDF, the code shows `age = “20”`, `print(“name”)` and `print(“age”)` (with curly quotes), but the answer says the output is *Ali and 20*. That code would actually print `name` and `age` (and curly quotes cause a syntax error in Python). The notebook uses the correct version from slide 6.

---

⬅️ [Previous lesson](../day-02-variables-data-types-and-input/) · [🏠 Course home](../../README.md) · [Next lesson ➡️](../day-04-while-loops/)
