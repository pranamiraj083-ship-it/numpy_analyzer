Numpy-Analyzer

A menu-driven, interactive command-line tool for creating, exploring, and analyzing NumPy arrays. Built entirely with Python and NumPy, it walks you through array creation, indexing/slicing, mathematical operations, combining/splitting, searching/sorting/filtering, and statistical analysis — all through a simple console interface.

Features
Array Creation — Build 1D, 2D, or 3D arrays by entering custom dimensions and elements
Indexing & Slicing — Access individual elements or extract sub-arrays across any dimension
Mathematical Operations — Add, subtract, multiply, or divide two arrays of the same shape
Combine or Split Arrays — Stack/concatenate arrays together or split an array into multiple parts
Search, Sort & Filter — Locate values, sort arrays (row-wise for 2D), or filter elements by condition
Aggregates & Statistics — Compute sum, mean, median, standard deviation, and variance
Project Structure
 Jupyter/
│   └── numpy_A.ipynb    # Main notebook containing the NumPy Analyzer program
└──----- README.md
Requirements
Python 3.x
NumPy
Installation
Clone the repository:

git clone https://github.com/pranamiraj083-ship-it/numpy_analyzer.git
cd Numpy-Analyzer
Install the required dependency:

pip install numpy
Usage
Open and run Jupyter/numpy_A.ipynb in Jupyter Notebook / JupyterLab, or convert it to a script and run it from the terminal.

On launch, you'll see the main menu:

Welcome to the NumPy Analyzer!
======================================

Choose an option:
1. Create a NumPy Array
2. Perform Mathematical Operations
3. Combine or Split Arrays
4. Search, Sort, or Filter Arrays
5. Compute Aggregates and Statistics
6. Exit
Simply enter the number corresponding to the operation you'd like to perform, then follow the on-screen prompts to input array dimensions and values.

Example Workflow
Select 1 to create a new array (choose 1D, 2D, or 3D and enter its elements)
Immediately after creation, you can index or slice the array
Return to the main menu and select 2–5 to perform further operations on the same array
How It Works
The program is organized into modular functions, each handling one category of operations:

Function	Purpose
create_array()	Builds a 1D, 2D, or 3D array from user input
indexing_slicing()	Retrieves elements or sub-arrays via indexing/slicing
mathematical_operations()	Performs element-wise arithmetic between two arrays
combine_split()	Combines two arrays or splits one into parts
search_sort_filter()	Searches, sorts, or filters array values
aggregates_statistics()	Calculates summary statistics for the array
main()	Drives the top-level menu loop
Notes
2D arrays are sorted row-wise by default.
When combining two 2D arrays, they are joined using a vertical stack (np.vstack).
Mathematical operations and combining arrays require the second array to match the shape of the original.
License
This project is open source and available for personal and educational use.


  
