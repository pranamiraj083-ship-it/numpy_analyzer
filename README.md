# NumPy Analyzer

A command-line / Jupyter Notebook tool for creating and exploring NumPy arrays interactively. It lets you build 1D, 2D, or 3D arrays and then run indexing, slicing, mathematical operations, combining/splitting, searching/sorting/filtering, and statistical aggregates on them — all through simple, menu-driven prompts.

## Table of Contents

- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Example Session](#example-session)
- [Project Structure](#project-structure)
- [Notes](#notes)
- [License](#license)

## Features

- **Array Creation** — Build a 1D, 2D, or 3D NumPy array by entering its dimensions and elements.
- **Indexing & Slicing** — Access single elements or sub-arrays across any supported dimensionality.
- **Mathematical Operations** — Add, subtract, multiply, or divide your array with another array of the same shape.
- **Combine or Split Arrays** — Stack/concatenate two arrays together, or split one array into multiple parts.
- **Search, Sort, and Filter** — Find a value's position, sort the array (row-wise for 2D), or filter elements above a threshold.
- **Aggregates & Statistics** — Compute sum, mean, median, standard deviation, and variance.

## Requirements

- Python 3.x
- [NumPy](https://numpy.org/)
- Jupyter Notebook (to run the `.ipynb` file)

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/pranamiraj083-ship-it/numpy_analyzer.git
   cd numpy_analyzer
   ```

2. Install the required dependency:

   ```bash
   pip install numpy
   ```

3. (Optional) Install Jupyter if you don't already have it:

   ```bash
   pip install notebook
   ```

## Usage

Open and run the notebook:

```bash
jupyter notebook jupyter/numpy_analyzer.ipynb
```

Run the cells to launch the interactive menu. You'll be greeted with a main menu:

```
1. Create a NumPy Array
2. Perform Mathematical Operations
3. Combine or Split Arrays
4. Search, Sort, or Filter Arrays
5. Compute Aggregates and Statistics
6. Exit
```

Start by choosing **1** to create an array, then use the other options to operate on it. Sub-menus will prompt you for the specific inputs needed (dimensions, elements, index/slice ranges, etc.).

## Example Session

```
Enter your choice: 1

Array Creation:
Select the type of array to create:
1. 1D Array
2. 2D Array
3. 3D Array
Enter your choice: 1

Enter the number of elements: 5
Enter 5 elements separated by space: 10 20 30 40 50

Array created successfully:
[10 20 30 40 50]

Choose an operation:
1. Indexing
2. Slicing
3. Go Back
Enter your choice: 2

Enter the start index: 1
Enter the end index: 4

Sliced Array:
[20 30 40]
```

## Project Structure

```
numpy_analyzer/
└── jupyter/
    ├── numpy_analyzer.ipynb   # Main notebook containing the interactive analyzer
    └── README.md              # This file
```

## Notes

- Mathematical operations and array combining require entering a second array with the same shape as the original.
- Splitting uses `np.array_split`, so parts may have uneven sizes if the array doesn't divide evenly.
- Sorting on 2D arrays is applied row-wise.

## License

This project is open source and available for personal and educational use.

## Author

**Repository:** [pranamiraj083-ship-it/numpy_analyzer](https://github.com/pranamiraj083-ship-it/numpy_analyzer.git)
