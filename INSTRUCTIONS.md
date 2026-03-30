# Instructions

## Setup Instructions

1. Clone the repository to your computer:
   ```bash
   git clone https://github.com/orassayag/styled-budgety-calculator.git
   cd styled-budgety-calculator
   ```

2. Open `index.html` in your web browser:
   - **Option 1**: Double-click `index.html` to open in your default browser
   - **Option 2**: Right-click `index.html` → Open With → Choose your browser
   - **Option 3**: Use a local development server (recommended for development):
     ```bash
     # Using Python 3
     python -m http.server 8000
     
     # Using Node.js http-server
     npx http-server
     ```

## How to Use

### Adding Income or Expenses

1. **Select the type**:
   - Click the dropdown and choose `+` for income or `-` for expense

2. **Enter description**:
   - Type a description for the item (e.g., "Salary", "Rent", "Groceries")

3. **Enter value**:
   - Type the amount (numbers only, no currency symbols)

4. **Add the item**:
   - Click the green checkmark button or press `Enter`

### Viewing Your Budget

The top section displays:
- **Available Budget**: Total income minus total expenses
- **Income**: Total income with green background
- **Expenses**: Total expenses with red background and percentage of income

### Managing Items

- **Delete an item**: Hover over any item in the list and click the `×` button that appears
- **View percentages**: Each expense shows what percentage it represents of your total income

### Visual Feedback

- The interface changes color based on whether you're adding income (green) or expenses (red)
- Items are displayed in separate lists for income and expenses
- All values are automatically formatted with commas and two decimal places

## Project Structure

```
styled-budgety-calculator/
├── index.html          # Main HTML file with structure
├── style.css           # All styles and layout
├── app.js              # Application logic
└── README.md           # Project documentation
```

## Code Architecture

The application uses the **Module Pattern** with three main controllers:

### 1. Budget Controller (`budgetController`)
Manages all budget-related data and calculations:
- Stores income and expense items
- Calculates totals and percentages
- Provides methods to add/delete items

### 2. UI Controller (`UIController`)
Handles all user interface operations:
- Gets input from form fields
- Displays items in lists
- Updates budget display
- Manages visual feedback

### 3. Global App Controller (`controller`)
Coordinates between Budget and UI controllers:
- Sets up event listeners
- Orchestrates data flow
- Updates UI when data changes

## Browser Compatibility

This application works in all modern browsers:
- Chrome (recommended)
- Firefox
- Safari
- Edge

**Requirements:**
- JavaScript must be enabled
- ES6 support (all modern browsers)

## Customization

### Changing Colors

Edit `style.css`:
- Income color: `#28B9B5` (teal)
- Expense color: `#FF5049` (red)

### Modifying Functionality

Edit `app.js`:
- Budget calculations are in `budgetController`
- UI rendering is in `UIController`
- Event handling is in `controller`

## Development

### File Descriptions

**index.html**:
- Single-page application structure
- Includes form for input
- Sections for income and expense lists
- Links to external CSS and JavaScript

**style.css**:
- Responsive design
- Separate styling for income and expenses
- Hover effects and transitions
- Font: Open Sans from Google Fonts

**app.js**:
- ES6 JavaScript with Module Pattern
- Three separate modules (controllers)
- IIFE (Immediately Invoked Function Expression) for encapsulation
- No external dependencies

### Testing

1. **Add income items** and verify:
   - Budget increases
   - Items appear in income list
   - Values are formatted correctly

2. **Add expense items** and verify:
   - Budget decreases
   - Expense percentage is calculated
   - Items appear in expense list

3. **Delete items** and verify:
   - Budget recalculates
   - Items are removed from lists
   - Percentages update

4. **Edge cases**:
   - Empty description (should not add)
   - Zero or negative value (should not add)
   - Delete all items (should show 0 budget)

## Notes

- No server or backend required
- All data is stored in memory (page refresh clears data)
- No external dependencies or frameworks
- Pure vanilla JavaScript ES6
- Responsive design (works on different screen sizes)

## Author

* **Or Assayag** - *Initial work* - [orassayag](https://github.com/orassayag)
* Or Assayag <orassayag@gmail.com>
* GitHub: https://github.com/orassayag
* StackOverflow: https://stackoverflow.com/users/4442606/or-assayag?tab=profile
* LinkedIn: https://linkedin.com/in/orassayag
