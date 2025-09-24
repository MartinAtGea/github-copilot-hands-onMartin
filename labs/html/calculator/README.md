# Interactive Calculator Lab 🧮

In this hands-on lab, you'll build a fully functional calculator with a clean interface using HTML, CSS, and JavaScript with the help of GitHub Copilot! This lab demonstrates how GitHub Copilot can assist with creating interactive web applications.

## Lab Overview 📋

**Duration**: 30-45 minutes  
**Difficulty**: Beginner  
**Prerequisites**: Basic knowledge of HTML, CSS, and JavaScript  

## What You'll Build 🏗️

A modern calculator with the following features:

- Clean, responsive design with a grid-based button layout
- Support for basic arithmetic operations (+, -, *, /)
- Keyboard input support (users can type numbers and operations directly)
- Enter key functionality for calculations
- Clear button to reset the display
- Input validation to allow only valid calculator inputs
- Error handling for invalid expressions

![Calculator Preview](calculator-preview.png)

## Requirements 💻

- IDE, e.g. Visual Studio Code
- [Live Server extension](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
- Web browser

## Getting Started 🚀

### Step 1: Create the HTML Structure

Start by creating a new file called `calculator.html` and ask GitHub Copilot to help you create the basic structure.

!!! tip "Copilot Tip"
    Try typing a comment like `<!-- Create a calculator with a display and number/operation buttons -->` and let Copilot generate the initial HTML structure.

**Prompt for Copilot:**
```html
<!-- Create a calculator with a display input field and buttons for numbers 0-9, operations +, -, *, /, equals =, and clear C -->
```

??? abstract "Sample HTML Structure"
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>Calculator</title>
    </head>
    <body>
      <div class="calculator">
        <input type="text" class="display" id="display">
        <div class="buttons">
          <button class="button" onclick="appendValue('7')">7</button>
          <button class="button" onclick="appendValue('8')">8</button>
          <button class="button" onclick="appendValue('9')">9</button>
          <button class="button" onclick="appendValue('/')">/</button>
          <!-- More buttons... -->
        </div>
      </div>
    </body>
    </html>
    ```

### Step 2: Style the Calculator

Add CSS to make the calculator look modern and appealing.

!!! tip "Copilot Tip"
    Use comments to describe the styling you want: `/* Style the calculator with a modern design, centered on page */`

**Prompt for Copilot:**
```css
/* Style the calculator with:
   - Centered layout on the page
   - Clean white background with shadow
   - Grid layout for buttons
   - Blue buttons with hover effects
   - Red clear button
*/
```

Key CSS features to implement:
- Flexbox centering for the calculator
- CSS Grid for button layout
- Hover effects for buttons
- Responsive design
- Clean typography

### Step 3: Add Basic JavaScript Functionality

Implement the core calculator functions.

!!! tip "Copilot Tip"
    Start with a comment describing each function: `// Function to append values to the display`

**Prompts for Copilot:**
```javascript
// Function to append values to the display
function appendValue(value) {
    // Add the value to the display
}

// Function to clear the display
function clearDisplay() {
    // Clear the display field
}

// Function to calculate the result
function calculate() {
    // Evaluate the expression and show result
}
```

### Step 4: Add Keyboard Input Support

Enhance the calculator to accept keyboard input.

!!! tip "Copilot Tip"
    Use a comment like: `// Add event listener for keyboard input to allow typing`

**Prompt for Copilot:**
```javascript
// Add event listener to allow users to type numbers and operators directly
// Also allow Enter key to calculate the result
```

### Step 5: Add Input Validation

Implement validation to ensure only valid calculator inputs are accepted.

!!! tip "Copilot Tip"
    Comment your validation needs: `// Validate input to allow only numbers, operators, and decimal points`

**Prompt for Copilot:**
```javascript
// Function to validate input - only allow numbers, +, -, *, /, and decimal points
function validateInput() {
    // Remove any invalid characters from the display
}
```

### Step 6: Add Error Handling

Make the calculator robust by handling calculation errors.

!!! tip "Copilot Tip"
    Use try-catch blocks: `// Handle calculation errors with try-catch`

## Features Explained 🔍

### 1. HTML Structure
- **Display Input**: Text input field where numbers and operations are shown
- **Button Grid**: 4x4 grid layout containing all calculator buttons
- **Semantic Elements**: Proper HTML structure for accessibility

### 2. CSS Styling
- **Responsive Design**: Calculator adapts to different screen sizes
- **Grid Layout**: CSS Grid for organized button placement
- **Modern UI**: Clean design with shadows and hover effects
- **Color Scheme**: Blue buttons for operations, red for clear

### 3. JavaScript Functionality
- **appendValue()**: Adds clicked button values to display
- **clearDisplay()**: Resets the calculator display
- **calculate()**: Evaluates mathematical expressions using `eval()`
- **validateInput()**: Filters out invalid characters
- **Event Listeners**: Keyboard support including Enter key

### 4. User Experience Features
- **Keyboard Input**: Users can type directly into the calculator
- **Enter Key**: Press Enter to calculate results
- **Input Validation**: Only valid calculator characters are allowed
- **Error Handling**: Shows "Error" for invalid calculations

## Testing Your Calculator 🧪

1. **Test Button Clicks**: Click each button to ensure values appear correctly
2. **Test Keyboard Input**: Type numbers and operators directly
3. **Test Enter Key**: Press Enter after typing an expression
4. **Test Calculations**: Try various mathematical expressions:
   - Simple: `2 + 2`
   - Complex: `10 * 5 - 3`
   - Decimals: `3.14 * 2`
5. **Test Error Cases**: Try invalid expressions like `5 / 0` or `2 + +`
6. **Test Clear Function**: Use the C button to reset

## Running the Calculator 🚀

1. Save your `calculator.html` file
2. Right-click the file in VS Code
3. Select "Open with Live Server"
4. The calculator will open in your browser

You can now use your calculator by:
- Clicking buttons with your mouse
- Typing directly on your keyboard
- Pressing Enter to calculate results

## Common GitHub Copilot Prompts 💡

Here are some effective prompts you can use with GitHub Copilot when building this calculator:

- `// Create a modern calculator interface with CSS Grid`
- `// Add keyboard event listeners for calculator input`
- `// Implement calculation function with error handling`
- `// Style calculator buttons with hover effects`
- `// Validate user input to allow only valid calculator characters`
- `// Add Enter key functionality to calculate results`

## Bonus Challenges 🌟

If you have extra time, try these enhancements:

1. **Memory Functions**: Add M+, M-, MR, MC buttons
2. **History**: Show previous calculations
3. **Advanced Operations**: Add square root, percentage, etc.
4. **Themes**: Add dark/light mode toggle
5. **Sound Effects**: Add button click sounds
6. **Keyboard Shortcuts**: Add more keyboard shortcuts

## Troubleshooting 🔧

**Calculator not working?**
- Check that all function names match between HTML onclick and JavaScript
- Ensure the display element ID matches your JavaScript selectors
- Verify Live Server is running for local testing

**Keyboard input not working?**
- Make sure event listeners are properly attached to the display element
- Check that the validateInput function is called on the right event

**Styling issues?**
- Verify CSS Grid properties are correctly applied to the buttons container
- Check that CSS selectors match your HTML class names

## Resources 📚

- [MDN Web Docs - CSS Grid](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout)
- [MDN Web Docs - JavaScript Events](https://developer.mozilla.org/en-US/docs/Web/API/Event)
- [GitHub Copilot Documentation](https://docs.github.com/en/copilot)
- [Reference Implementation](https://github.com/ps-copilot-sandbox/javascript-calculator-demo)