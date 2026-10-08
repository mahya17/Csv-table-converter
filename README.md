# CSV Table Converter 🍕

A Python program that reads a CSV file containing pizza menu data and converts it into a formatted ASCII table.

## About the Project

The program takes the path to a CSV file as a command-line argument, reads the pizza menu data, and displays it as an ASCII table using the `tabulate` package.

The program also checks the command-line arguments and handles invalid file names and missing files.

## How It Works

The program expects exactly one command-line argument containing the path to a CSV file.

For example:

```bash
python pizza.py sicilian.csv
```

The CSV data is read using Python's `csv` module and then formatted as an ASCII table with `tabulate`.

The table uses the `grid` format.

## Error Handling

The program exits with an error message when:

* No command-line argument is provided
* More than one command-line argument is provided
* The file does not have a `.csv` extension
* The specified file does not exist

Example:

```text
Too few command-line arguments
Too many command-line arguments
Not a CSV file
File does not exist
```

## What I Practiced

* Command-line arguments
* `sys.argv`
* `sys.exit()`
* Reading CSV files
* `csv.DictReader`
* File handling
* Exception handling
* `FileNotFoundError`
* Using external Python packages
* Formatting data with `tabulate`

## Technologies

* Python
* CSV
* tabulate

## Installation

Install the `tabulate` package with:

```bash
pip install tabulate
```

## Course

This project was completed as part of **CS50's Introduction to Programming with Python** by Harvard University.
