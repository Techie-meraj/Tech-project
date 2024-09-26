
This project is a simple JavaScript calculator embedded in an HTML file. It features basic mathematical operations such as addition, subtraction, multiplication, division, and includes additional functionality for clearing the display, deleting the last character, and evaluating the inputted expression.

Structure Breakdown
HTML Structure:

The HTML file defines a basic calculator interface inside a container <div> with buttons for numbers, operators, and control functions like clearing the screen and evaluating results.
A <form> is used to group input buttons and an input field, which serves as the display for the calculator.
Each button corresponds to a number, an operator, or a function (like clearing or deleting a character). The button's value attribute is used to display the text, and the onclick attribute is linked to JavaScript functions that handle the button's functionality.
JavaScript Functions:

calnum(value): This function is called when any number or operator button is clicked. It retrieves the current value of the textarea (the display screen) and updates it with the clicked button's value.
clearscreen(): This function clears the textarea, effectively resetting the display.
dellastchr(): This function removes the last character in the textarea. The slice(0, -1) method is used to remove the last character from the current string displayed on the screen.
calresult(): This function evaluates the expression entered in the textarea using the JavaScript eval() function. It calculates the result of the mathematical expression and updates the textarea with the result.

Key Functionalities:

Display Input (textarea): All user input (numbers and operators) is displayed in the input field (<input type="text" id="textarea">), which acts as the calculator's display.
Number and Operator Input: Clicking on buttons updates the display with the respective numbers or operators using the calnum() function.
Delete Last Character: Clicking the "DE" button calls the dellastchr() function, which removes the last character from the current input.
Clear Screen: Clicking the "AC" button clears the entire input using the clearscreen() function.
Calculate Result: Clicking the "=" button evaluates the expression and displays the result using the calresult() function.

How it Works

When a user clicks any number or operator, the calnum() function captures the value and updates the display by setting it as the value of the input field (textarea).
The clearscreen() function completely clears the input field when the "AC" button is pressed.
The dellastchr() function slices off the last character of the input string whenever the "DE" button is clicked.
The calresult() function uses JavaScript's eval() function to calculate the result of the inputted expression when the "=" button is clicked, and updates the display with the result.

Project Features:

Basic Arithmetic: Supports addition, subtraction, multiplication, and division.
Clear Function: Resets the display to an empty value when "AC" is clicked.
Delete Function: Removes the last character typed into the display.
Real-time Calculation: Uses the eval() function to calculate the expression entered by the user when "=" is clicked.
