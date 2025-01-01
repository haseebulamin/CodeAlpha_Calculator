# Simple Calculator

A minimalistic calculator built using HTML and CSS, with a touch of inline JavaScript for basic arithmetic operations. This project is perfect for beginners looking to explore web development basics.

## Features
- Basic arithmetic operations: addition, subtraction, multiplication, and division.
- Intuitive and simple user interface.
- Lightweight and responsive design.

## Demo
Open the `index.html` file in any web browser to see the calculator in action.

## Technologies Used
- **HTML**: For the structure of the calculator.
- **CSS**: For styling the calculator.
- **JavaScript**: For adding basic functionality.

## File Structure
```
Simple-Calculator/
├── index.html       # Main HTML file containing the calculator structure and inline JS.
├── style.css        # External CSS file for styling.
└── README.md        # Documentation (this file).
```

## How to Use
1. Clone or download the repository.
2. Open the `index.html` file in your preferred web browser.
3. Use the buttons on the calculator to perform arithmetic operations.

## Code Overview
### HTML
The structure of the calculator, including buttons and display.
```html
<div class="calculator">
  <input type="text" id="display" disabled />
  <div class="buttons">
    <button onclick="appendValue('1')">1</button>
    <button onclick="appendValue('2')">2</button>
    <!-- More buttons -->
    <button onclick="calculate()">=</button>
  </div>
</div>
```

### CSS
Basic styling for layout and button design.
```css
.calculator {
  width: 300px;
  margin: auto;
  padding: 20px;
  border: 1px solid #ccc;
  border-radius: 10px;
  text-align: center;
}
```

### JavaScript
Inline functions for calculator operations.
```javascript
function appendValue(value) {
  document.getElementById('display').value += value;
}

function calculate() {
  try {
    document.getElementById('display').value = eval(document.getElementById('display').value);
  } catch (e) {
    alert('Invalid operation');
  }
}
```

## Future Enhancements
- Add support for advanced operations (e.g., square root, percentage).
- Include better error handling.
- Transition to external JavaScript for improved modularity.

## License
This project is open-source and available under the [MIT License](LICENSE).

---

Enjoy calculating! 😊
