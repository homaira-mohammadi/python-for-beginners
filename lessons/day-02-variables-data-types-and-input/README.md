# Day 2 — Variables, Data Types, Input & Operators

⏱️ **Duration:** 90–120 minutes  ·  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/homaira-mohammadi/python-for-beginners/blob/main/lessons/day-02-variables-data-types-and-input/lesson.ipynb)

Students learn how Python *remembers* information with variables, the four basic data types, how to get input from the user and how to do maths with operators.

## 🎯 Learning objectives

- Create, name and update variables
- Recognise `int`, `float`, `str` and `bool`
- Check types with `type()`
- Get user input with `input()`
- Convert types with `int()`, `float()`, `str()`
- Use `+ - * / // % **`
- Combine text and variables with commas and f-strings

## 📁 Files in this lesson

| File | What it is |
|---|---|
| [`slides/Day-02-Variables-and-Data-Types.pdf`](slides/Day-02-Variables-and-Data-Types.pdf) | Slides (view on GitHub) |
| [`slides/Day-02-Variables-and-Data-Types.pptx`](slides/Day-02-Variables-and-Data-Types.pptx) | Slides (PowerPoint, for teaching) |
| [`lesson.ipynb`](lesson.ipynb) | 📘 The full lesson — explanations + code you can run |
| [`exercises.ipynb`](exercises.ipynb) | ✏️ Exercises for students (empty code cells) |
| [`solutions.ipynb`](solutions.ipynb) | ✅ Example solutions with output |

## 🧠 Key concepts

| Concept | Explanation |
|---|---|
| Variable | A labelled box that stores a value: `name = "Ali"`. `=` means *assign*, not *equals*. |
| Naming rules | No leading numbers, no spaces, case-sensitive. Use `snake_case`: `student_age`. |
| Data types | `int` 10 · `float` 3.5 · `str` "Python" · `bool` True |
| `input()` | Always returns a **string** — convert it with `int()` or `float()` before doing maths. |
| Operators | `//` whole-number division, `%` remainder, `**` power |
| f-strings | `f"I am {age} years old"` |

## 🧑‍🏫 Suggested class plan

| Time | Activity |
|---|---|
| 10 min | Review of Day 1 |
| 20 min | Why variables? Creating variables, naming rules, good names |
| 10 min | Multiple assignment and changing values |
| 15 min | Data types and `type()` |
| 15 min | Arithmetic operators (`//`, `%`, `**`) and order of operations |
| 20 min | `input()` and type conversion |
| 10 min | Combining text and variables; f-strings |
| 15 min | Let's code together + simple calculator |

## ✨ Added in this improved version

Compared to the original slides, the notebook adds:

- `type()` to check data types
- `input()` and type conversion — Day 3's review and examples rely on these, but they weren't in the slides
- All arithmetic operators incl. `//`, `%` (needed for *even/odd* on Day 3) and `**`
- `+=` shortcuts, order of operations
- Commas vs `+` vs f-strings for combining text and variables
- Quick-check questions and 10 exercises incl. a *shopping receipt* mini project

## 📌 Note

The last two slides in the original deck were empty, so they've been left as they are. The notebook covers the extra topics.

---

⬅️ [Previous lesson](../day-01-introduction-to-python/) · [🏠 Course home](../../README.md) · [Next lesson ➡️](../day-03-conditional-statements/)
