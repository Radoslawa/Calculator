# Simple JavaScript Calculator

This repository contains a simple calculator web application built with HTML, CSS, and JavaScript.

## Project Description

This project is a basic calculator that allows users to perform arithmetic operations. It features a clean and user-friendly interface with buttons for numbers, operators, and functions like clear and equals.

## Features

* **Basic Arithmetic Operations:** Addition, subtraction, multiplication, and division.
* **Clear Functionality:** Clears the display.
* **Error Handling:** Displays "Error" when an invalid calculation is attempted.
* **Responsive Design:** The calculator is designed to be user-friendly on various screen sizes.
* **Simple and Clean UI:** The calculator has a straightforward and easy-to-use interface.

## Technologies Used

* **HTML:** For structuring the calculator's layout.
* **CSS:** For styling the calculator's appearance.
* **JavaScript:** For handling the calculator's functionality.

## Getting Started

To run the calculator on your local machine, follow these steps:

1.  **Clone the Repository:**
    ```bash
    git clone [repository URL]
    ```
2.  **Open `index.html`:** Open the `index.html` file in your web browser.

## Files Included

* **`index.html`:** The main HTML file for the calculator.
* **`index.js`:** The JavaScript file containing the calculator's logic.
* **`styles.css`:** The CSS file for styling the calculator.

## JavaScript Code Explanation

```javascript
const display = document.getElementById("display");

function appendToDisplay(input) {
    display.value += input;
}

function clearDisplay() {
    display.value = "";
}

function calculate() {
    try {
        display.value = eval(display.value);
    } catch (error) {
        display.value = "Error";
    }
}
