# 🗂️ GitHub Guide: Uploading and Maintaining This Course

This page explains how the repository is organised and how to upload or update it.

---

## 1. How the repository is organised

- **One folder per lesson** inside `lessons/`, named `day-XX-topic` (with a leading zero so they sort correctly: `day-01` … `day-10`).
- **Every lesson folder has the same files**: `README.md`, `slides/`, `lesson.ipynb`, `exercises.ipynb`, `solutions.ipynb`.
- **Slides are stored twice**: as a **PDF** (GitHub shows PDFs right in the browser) and as **PowerPoint** (for editing and teaching).
- **Shared material** (setup, cheat sheet, next steps) lives in `resources/`.
- **File names** use lowercase and dashes, with no spaces: `day-03-conditional-statements`, not `Day 3 Conditional Statements`.

---

## 2. Uploading for the first time (no Git needed)

1. Sign in to [github.com](https://github.com) → click **+** (top right) → **New repository**.
2. Name: `python-for-beginners` · Description: *A complete beginner-friendly Python course* · choose **Public** · ❌ don't add a README (we have one).
3. Click **Create repository**.
4. On the next page, click **uploading an existing file**.
5. Unzip the course folder on your computer, open it, select **everything inside** (`README.md`, `lessons`, `resources`, …) and **drag it** into the browser.
6. Write a message like `Add Python for Beginners course` and click **Commit changes**.

> ⚠️ The web uploader has a limit of 100 files per upload. This course has fewer, so one upload is enough.
> ⚠️ Hidden files like `.gitignore` may not be selected by drag-and-drop on Mac. That's okay, it's optional.

### Uploading with Git (if you have it installed)
```bash
cd python-for-beginners
git init
git add .
git commit -m "Add Python for Beginners course"
git branch -M main
git remote add origin https://github.com/homaira-mohammadi/python-for-beginners.git
git push -u origin main
```

---

## 3. Make the repo look professional ✨

On the repository's main page:
1. Click the ⚙️ next to **About** (right side) → add a description, and **topics** such as `python`, `python-course`, `beginners`, `jupyter-notebook`, `teaching`.
2. Optional: add a **license** (*Add file → Create new file*, name it `LICENSE`, then click *Choose a license template*). **CC BY 4.0** is common for course material, and **MIT** for code.
3. Optional: pin the repository to your GitHub profile (*Profile → Customize your pins*).

---

## 4. Updating the course later

| I want to… | How (on github.com) |
|---|---|
| Fix a typo in a README | Open the file → ✏️ pencil icon → edit → **Commit changes** |
| Replace a notebook | Open the lesson folder → **Add file → Upload files** → upload the file with the **same name** → commit |
| Add slides to Day 4 | Open `lessons/day-04-while-loops/` → **Add file → Upload files** → name it `slides/Day-04-While-Loops.pdf` |
| Add a new lesson | Create a folder `lessons/day-11-topic/` with the same 4 files, then add a row to the table in the main `README.md` |

### Good commit messages
Write short messages that describe the change:
- ✅ `Add slides for Day 4`
- ✅ `Fix typo in Day 2 exercises`
- ❌ `update` / `stuff`

---

## 5. Tips for the notebooks

- The **lesson** and **solutions** notebooks are saved **with their outputs**, so students can see results on GitHub without running anything.
- The **exercises** notebooks are saved **without outputs** (empty cells for students).
- If you edit a notebook in Colab, use **File → Save a copy in GitHub** to save it straight back to this repository.
- The **Open in Colab** badges in each lesson README point to `homaira-mohammadi/python-for-beginners`. If you rename the repository, update those links.
