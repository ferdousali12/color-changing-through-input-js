# 🎨 Dynamic Color Previewer

A simple, interactive web tool that changes the background color of a display box in real-time based on user input.

## 🚀 How it Works
The application uses an event listener on the input field. As the user types a valid CSS color name (e.g., "Red", "SkyBlue") or a Hex/RGB code, the JavaScript function dynamically updates the `backgroundColor` style property of the result box.

## 🛠️ Tech Stack
* **HTML5:** Structure of the interface.
* **CSS3:** Styling and layout.
* **JavaScript (ES6):** Logic for DOM manipulation and event handling.

## 💻 Code Snippet
```javascript
let inputBox = document.getElementById("input-box");
let resultBox = document.getElementById("result-box");

let changeColor = () => {
  let input = inputBox.value;
  resultBox.style.backgroundColor = input;
};

// Listen for typing events
inputBox.addEventListener("input", changeColor);

// Ensure the color is set on initial page load
window.addEventListener("load", changeColor);
