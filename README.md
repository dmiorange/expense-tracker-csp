# Expense Tracker - AP CSP Create Performance Task

My program lets a user log daily expenses by category, track their total spending against a monthly budget, and visualize a breakdown of where their money goes.

## About This Project

This app was built as my **AP Computer Science Principles Create Performance Task**. The goal of the Create PT is to design and program an app that demonstrates key programming concepts including lists, functions with parameters, algorithms, and user input/output.

## Features

- Add expenses by category (Food, Transport, Entertainment, Shopping, Utilities, Other)
- Live spending breakdown showing total spent and budget remaining
- Recent expenses list showing the last 5 entries
- Pie chart visualization of spending by category
- Settings to change currency (USD, EUR, GBP) and set a monthly budget

## How to Use

1. Open the app and click **Start Tracking**
2. Select a category, enter an amount, and optionally add a description
3. Click **Add Expense** - your breakdown updates instantly
4. Visit **Statistics** to see a pie chart of spending by category
5. Go to **Settings** to set a monthly budget or change your currency

## AP CSP Requirements Met

### List
The program stores all expenses in a list of objects:
```javascript
var expenses = [];
// Each entry: { category, amount, description }
```
This list is iterated over to calculate totals and display recent entries, making it easier to manage any number of expenses without rewriting code.

### Student-Developed Function
`displayBreakdown(expenseList)` meets all algorithm requirements:
- **Parameter** - accepts `expenseList` as input
- **Iteration** - loops through every expense to sum the total
- **Selection** - uses an `if` statement to check whether a budget has been set before displaying remaining balance
- **Sequencing** - multiple steps run in order to build and display the output string

### Input / Output
- **Input:** category dropdown, amount field, description field, settings controls
- **Output:** spending breakdown text, recent expenses list, pie chart

## Built With

- HTML, CSS, JavaScript
- [Chart.js](https://www.chartjs.org/) for pie chart visualization
- Originally developed in [Code.org App Lab](https://code.org/educate/applab)

## Acknowledgments

Chart.js library used for the statistics pie chart - all other code written by me during the administration of the task.
