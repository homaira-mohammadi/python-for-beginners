# 🛠️ Setup Guide

You can follow this course in **three ways**. Pick the one that suits you. If you're not sure, use **Google Colab**.

---

## Option 1: Google Colab ⭐ (recommended for beginners)

✅ Nothing to install · ✅ Works on any computer or Chromebook · ✅ Free

1. Make sure you're signed in to a Google account.
2. On any lesson page in this repository, click the **Open in Colab** badge:
   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](#)
3. The notebook opens in your browser.
4. Click **File → Save a copy in Drive** so you can keep your changes.
5. Click a code cell and press **Shift + Enter** to run it.

> 💡 The first time you run a cell, Colab may take a few seconds to start.

---

## Option 2: VS Code (for working on your own computer)

### Step 1: Install Python
1. Go to [python.org/downloads](https://www.python.org/downloads/) and download the latest Python 3.
2. Run the installer.
   ⚠️ **Windows:** tick the box **"Add Python to PATH"** before clicking *Install Now*.
3. Check that it worked. Open a terminal (Command Prompt on Windows, Terminal on Mac) and type:
   ```
   python --version
   ```
   (on Mac you may need `python3 --version`). You should see something like `Python 3.13.0`.

### Step 2: Install VS Code
1. Download it from [code.visualstudio.com](https://code.visualstudio.com/).
2. Open VS Code → click the **Extensions** icon (four squares) on the left.
3. Install these two extensions:
   - **Python** (by Microsoft)
   - **Jupyter** (by Microsoft)

### Step 3: Get the course files
- On the GitHub page, click the green **Code** button → **Download ZIP**, then unzip it.
- *(Or, if you know Git: `git clone` the repository.)*

### Step 4: Open a notebook
1. In VS Code: **File → Open Folder** → choose the `python-for-beginners` folder.
2. Open any `lesson.ipynb`.
3. Click **Select Kernel** (top right) and choose your Python installation.
4. Run cells with **Shift + Enter**.

---

## Option 3: Python IDLE (simplest editor)

IDLE comes with Python (installed in Option 2, Step 1).

1. Open **IDLE** from your Start menu / Applications.
2. Type code directly after `>>>` and press Enter, **or**
3. Click **File → New File**, write a program, save it as `something.py`, and press **F5** to run it.

> ℹ️ IDLE can't open `.ipynb` notebooks. Copy the code from the notebook on GitHub into IDLE.

---

## Running the notebooks with Jupyter (optional)

If you prefer the classic Jupyter interface:
```
pip install -r requirements.txt
jupyter notebook
```
This opens Jupyter in your browser. Then click a lesson folder → `lesson.ipynb`.

---

## ❓ Common problems

| Problem | Fix |
|---|---|
| `python` is not recognised (Windows) | Re-install Python and tick **Add Python to PATH** |
| VS Code asks for a kernel | Click **Select Kernel → Python Environments** and choose Python 3 |
| A cell keeps running forever | You have an infinite loop. Press the **■ Stop** button (or *Interrupt*) |
| A cell with `input()` is waiting | Type your answer in the box that appears and press **Enter** |
| `NameError` for a variable that exists | Run the cells **above** first. Notebooks remember cells in the order you run them |
