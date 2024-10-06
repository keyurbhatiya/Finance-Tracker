# Finance-Tracker

# Finance Data Manager

A simple Python project for managing personal finances by adding, viewing, and plotting transactions. The project uses CSV files to store data and provides options to filter transactions based on date ranges, view summaries, and plot income vs expenses over time.

## Features

- Add new transactions (income or expenses) with date, amount, category, and description.
- View transactions within a specified date range.
- Get a summary of total income, expenses, and net savings.
- Visualize transactions with a time-based plot (Income vs. Expenses).
- Data is stored in a CSV file for easy access and modification.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/keyurbhatiya/Finance-Tracker.git
    cd Finance-Tracker
    ```

2. Install required dependencies:
    ```bash
    pip install pandas matplotlib
    ```

3. (Optional) Install any additional dependencies for date entry:
    ```bash
    pip install datetime
    ```

## Usage

### Add a Transaction

To add a new transaction, run the program and follow the prompts to input the transaction details such as date, amount, category, and description.

```bash
python main.py
```

Example of adding a new transaction:
- Date: 05-10-2024
- Amount: 120.00
- Category: Income
- Description: Freelance work

### View Transactions and Summary

You can also view transactions within a specific date range and get a summary of total income, total expenses, and net savings. You can choose to visualize the data with a plot.

```bash
python main.py
```

You will be prompted to enter the start and end dates in the format `dd-mm-yyyy`, after which the program will display the transactions and offer an option to show a plot.

### Plot Income vs. Expenses

The project includes a plotting feature that allows you to visualize the income and expenses over a given period. You will see a graph comparing both categories on a timeline.

## CSV Structure

The transactions are stored in a CSV file (`finance_data.csv`) with the following columns:

- **date**: The date of the transaction (dd-mm-yyyy)
- **amount**: The transaction amount (positive for income, negative for expenses)
- **category**: The category of the transaction (Income or Expense)
- **description**: A brief description of the transaction

## Example Data

Here’s an example of the CSV file structure:

```csv
date,amount,category,description
05-10-2024,93.8,Income,salary
06-10-2024,278.0,Expense,Zebronics Mouse
07-10-2024,150.5,Expense,Groceries
```

