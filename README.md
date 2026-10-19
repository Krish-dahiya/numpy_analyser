<div align="center">

<img src="assets/numpy-analyzer-banner.svg" alt="NumPy Analyzer — Python array toolkit" width="100%">

# 🔢 NumPy Analyzer

### A menu-driven Python project for creating, transforming, and analyzing NumPy arrays.

<p>
  <img src="https://img.shields.io/badge/Python-3.9%2B-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/NumPy-Array%20Computing-013243?style=for-the-badge&logo=numpy&logoColor=white" alt="NumPy">
  <img src="https://img.shields.io/badge/Project-PR--08-7C3AED?style=for-the-badge" alt="PR-08 Project">
  <img src="https://img.shields.io/badge/Level-Beginner%20Friendly-16A34A?style=for-the-badge" alt="Beginner friendly">
</p>

**Created by Krish Kumar Prajapat** · Python Learning Project

[Features](#-features) • [Demo](#-sample-run) • [Installation](#-installation) • [How It Works](#-how-it-works) • [Future Improvements](#-future-improvements)

</div>

---

## 📌 About the Project

**NumPy Analyzer** is a command-line, menu-driven application built with Python and NumPy. It brings common array operations together in one place, so a user can choose an operation from the menu and see the result in the terminal.

The project is designed to practise core NumPy concepts, including array creation, indexing, slicing, element-wise arithmetic, combining and splitting arrays, searching, sorting, filtering, and basic statistics.

> **Project goal:** make essential NumPy operations easy to explore through a simple interactive menu.

## ✨ Features

| Menu option | What it does | NumPy tools / concepts |
|---|---|---|
| **1. Create a NumPy Array** | Create 1D, 2D, or 3D arrays; explore indexing and slicing | `np.array()`, `reshape()`, indexing, slicing |
| **2. Mathematical Operations** | Add, subtract, multiply, or divide two arrays | `+`, `-`, `*`, `/`, `np.any()` |
| **3. Combine or Split Arrays** | Stack arrays vertically or split a 2D array vertically | `np.vstack()`, `np.vsplit()` |
| **4. Search, Sort, or Filter** | Find a value, sort array values, or filter values above a threshold | `np.where()`, `np.sort()`, Boolean filtering |
| **5. Aggregates and Statistics** | Calculate sum, mean, median, standard deviation, and variance | `np.sum()`, `np.mean()`, `np.median()`, `np.std()`, `np.var()` |
| **6. Exit** | Close the program | `break` |

## 🖼️ Project Visuals

### 1. Program workflow

![NumPy Analyzer workflow](assets/workflow.svg)

### 2. Main components

![NumPy Analyzer component diagram](assets/components.svg)

### 3. Example output

The program runs in the terminal. A typical session starts with this menu:

```text
Welcome to the NumPy Analyzer!
=======================================
Main Menu - Choose an option:
1. Create a NumPy Array
2. Perform Mathematical Operations
3. Combine or Split Arrays
4. Search, Sort, or Filter Arrays
5. Compute Aggregates and Statistics
6. Exit
Enter your choice:
```

*Tip: After running the program, capture a screenshot of your own terminal output and save it as `assets/terminal-demo.png` if you want to add a real project screenshot here.*

## 🧰 Built With

- **Python** — program logic, user input, conditions, and loops.
- **NumPy** — numerical arrays and array operations.
- **Terminal / Command Prompt** — interactive interface.

## 🚀 Installation

### 1. Check Python

Install Python 3.9 or later, then check the version:

```bash
python --version
```

On some systems, use:

```bash
python3 --version
```

### 2. Install NumPy

```bash
python -m pip install numpy
```

If your system uses `python3`, you can run:

```bash
python3 -m pip install numpy
```

### 3. Get the project files

Download or clone this repository, then open a terminal in the project folder.

```bash
git clone https://github.com/Krish-dahiya/numpy-analyzer.git
cd numpy-analyzer
```

> **Repository note:** Replace the example repository URL above with your actual GitHub repository URL if your repository uses a different name.

### 4. Run the program

Save the Python code as `numpy_analyzer.py`, then run:

```bash
python numpy_analyzer.py
```

On some systems:

```bash
python3 numpy_analyzer.py
```

## 💻 Sample Run

### Example: Create a 2D array

Choose option `1`, then choose `2` for a 2D array.

```text
Enter your choice: 1

Select the type of array to create:
1. 1D Array
2. 2D Array
3. 3D Array
Enter your choice: 2

Enter number of rows: 2
Enter number of columns: 3
Enter 6 elements: 1 2 3 4 5 6

Array created successfully:
[[1 2 3]
 [4 5 6]]
```

### Example: Calculate the sum

For the array above, the sum of all elements is:

```text
Sum: 21
```

## 🧠 How It Works

1. The program imports NumPy as `np`.
2. A `while` loop repeatedly displays the main menu.
3. The user enters a menu number.
4. `if` / `elif` statements route the choice to the selected operation.
5. NumPy performs the requested calculation or array transformation.
6. The result is displayed in the terminal.
7. Selecting **6. Exit** ends the loop.

### Main menu logic

![Menu logic diagram](assets/menu-logic.svg)

## 📚 What I Learned

By building this project, I practised:

- Creating 1D, 2D, and 3D NumPy arrays.
- Understanding array shapes with `reshape()`.
- Accessing array elements using indexing and slicing.
- Performing element-wise mathematical operations.
- Combining and splitting arrays.
- Searching, sorting, and filtering array data.
- Calculating descriptive statistics.
- Building an interactive command-line program with loops and conditions.
- Checking for division-by-zero values before dividing arrays.

## ⚠️ Notes and Current Limitations

- The current program expects numeric input in the requested format. Entering text where a number is expected can stop the program with an input error.
- Some menu options use `arr1`, `rows`, and `cols` created by the 2D-array workflow. For the smoothest demo, first create a **2D array** before choosing mathematical, combine/split, search/sort/filter, or statistics options.
- Indexing and slicing prompts are currently designed around row and column access, so they work best with a 2D array.
- For vertical splitting, the number of splits must be compatible with the number of rows.
- This is an educational project; it can be improved with stronger input validation and more flexible handling of 1D, 2D, and 3D arrays.

## 🔮 Future Improvements

Ideas for a next version:

- [ ] Validate menu input and handle invalid values without stopping the program.
- [ ] Keep a clearly defined current array and reuse it across menu options.
- [ ] Support operations for both 1D and 2D arrays where appropriate.
- [ ] Add horizontal stacking and splitting.
- [ ] Add reshape, transpose, minimum, maximum, and cumulative-sum options.
- [ ] Add unit tests for array operations.
- [ ] Add a graphical interface or a small web interface.
- [ ] Add real screenshots and a short demo GIF.

## 📁 Suggested Repository Structure

```text
numpy-analyzer/
├── numpy_analyzer.py
├── README.md
└── assets/
    ├── numpy-analyzer-banner.svg
    ├── workflow.svg
    ├── components.svg
    └── menu-logic.svg
```

## 🤝 Contributions

This is a learning project. Suggestions, bug reports, and improvements are welcome. If you fork the project, feel free to improve the input validation, add new NumPy operations, or enhance the interface.

## 👨‍💻 Author

**Krish Kumar Prajapat**  
Aspiring Data Scientist · Python Learner

- GitHub: [@Krish-dahiya](https://github.com/Krish-dahiya)

---

<div align="center">

### ⭐ If you find this project useful, consider giving the repository a star!

**Built with Python + NumPy**

</div>
