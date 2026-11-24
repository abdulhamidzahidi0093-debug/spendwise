```markdown
# SpendWise

SpendWise is a simple budgeting application that helps users keep track of their monthly budget and expenses.

## Improvements Made This Week

This week I made SpendWise interactive using JavaScript. Users can now enter a monthly budget and add different expenses. The dashboard automatically updates when new expenses are added.

## Conditionals

I used conditional statements to check the user's spending.

For example, if the user spends more than their budget, the application displays a warning. It also gives a different message when the user is getting close to their budget.

```javascript
if (total > budget) {
    budgetMessage.textContent = "You have exceeded your budget.";
} else if (total >= budget * 0.8) {
    budgetMessage.textContent = "Warning: You are getting close to your budget.";
}
```

## Arrays

I used an array to store multiple expense records.

```javascript
let expenses = [];
```

When the user adds an expense, it is added to the array using `push()`.

```javascript
expenses.push({
    name: name,
    amount: amount
});
```

This makes it possible to keep track of more than one expense.

## Loops

I used a `for...of` loop to go through the expenses stored in the array.

The loop adds all the expense amounts together so that the application can calculate the total amount spent.

## DOM Manipulation

I used JavaScript DOM manipulation to update the information shown on the webpage.

For example:

```javascript
totalSpent.textContent = "KSh " + total.toLocaleString();
```

This allows the total spending to appear directly on the dashboard without refreshing the page.

## Events

I used event listeners to respond to user actions.

For example, when the user clicks the Add Expense button, the application reads the expense information and adds it to the expense array.

```javascript
addExpenseButton.addEventListener("click", function () {
    // Add expense
});
```

## Challenges

One challenge I had was making sure the total spending was updated whenever a new expense was added.

I solved this by creating an `updateDashboard()` function. This function calculates the total, checks the budget, and updates the information displayed on the page.

Another challenge was understanding how arrays and loops work together. After practicing with several expenses, I understood how the loop could go through each expense and calculate the total.

## Technologies Used

- HTML
- CSS
- JavaScript
- GitHub
```
