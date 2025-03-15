# JavaScript Spreadsheet

A lightweight, functional programming-based spreadsheet application built with vanilla JavaScript.

## Overview

This project implements a web-based spreadsheet with basic spreadsheet functionality similar to Excel or Google Sheets. It's built using functional programming principles and vanilla JavaScript (no external libraries or frameworks).

## Features

- Grid-based spreadsheet UI with labeled columns (A-J) and rows (1-99)
- Formula evaluation using standard mathematical operators (+, -, *, /)
- Cell references (e.g., `=A1+B2`)
- Range references (e.g., `=SUM(A1:A10)`)
- Built-in functions:
  - `SUM`: Add all values in a range
  - `AVERAGE`: Calculate the average of values
  - `MEDIAN`: Find the median value
  - `EVEN`: Filter only even numbers
  - `SOMEEVEN`: Check if any value is even
  - `EVERYEVEN`: Check if all values are even
  - `FIRSTTWO`: Get first two values
  - `LASTTWO`: Get last two values
  - `HAS2`: Check if range contains the value 2
  - `INCREMENT`: Add 1 to each value
  - `RANDOM`: Generate random number between given bounds
  - `RANGE`: Create a range of numbers
  - `NODUPES`: Remove duplicate values

## Usage

1. Open `index.html` in your browser
2. Input values directly into cells
3. To use formulas, start with an equals sign (`=`)
4. Reference other cells by their coordinates (e.g., `=A1+B2`)
5. Use functions with parentheses (e.g., `=SUM(A1:A5)`)

## Formula Examples

- Basic arithmetic: `=5+10`, `=A1*B1`
- Cell references: `=A1+A2`
- Range references: `=SUM(A1:A10)`
- Nested functions: `=AVERAGE(NODUPES(A1:A10))`

## Technical Implementation

The spreadsheet is implemented using:

- Vanilla JavaScript with functional programming techniques
- CSS Grid for the spreadsheet layout
- Regular expressions for formula parsing
- Higher-order functions for formula evaluation

### Key Components

- `evalFormula`: Main function to evaluate formulas with cell references
- `applyFunction`: Processes and applies spreadsheet functions
- `infixEval`: Handles mathematical operations
- `highPrecedence`: Ensures proper order of operations (multiplication/division before addition/subtraction)

## Browser Compatibility

Works with modern browsers that support:
- CSS Grid
- ES6 features (arrow functions, template literals, etc.)
- Modern DOM APIs

## License

This project is open source and available for educational purposes.
