# MauiApp2
Todo List and Calculator Blazor Application
This Blazor application contains two components: Todo List and Calculator.

Todo List
The Todo List component allows users to add, delete, and move todo items between two lists: Todo and Done. Here's how to use it:

Enter a new todo item in the input field.
Click the "Add" button to add the item to the Todo list.
Check the checkbox next to a todo item to move it to the Done list.
Click the delete button next to an item to remove it from the list.
The component uses exception handling to validate user input and display error messages.

Code Overview
TodoItem class: Represents each todo item with properties for text and checkbox status.
newTodoText string: Holds the text of the new todo item.
todoItems and doneItems lists: Store the todo and done items, respectively.
AddTodo function: Adds a new todo item to the list after validating user input.
MoveToDone function: Moves a todo item to the done list.
DeleteItem function: Deletes an item from the todo or done list.
ContainsSpecialCharacters function: Checks if the input text contains special characters.
Calculator
The Calculator component allows users to perform basic arithmetic operations: addition, subtraction, multiplication, and division. Here's how to use it:

Enter the first and second numbers in the input fields.
Click the button for the desired operation.
The result will be displayed in the result input field.
Click the "Clear All" button to reset all fields.
The component uses exception handling to validate user input and display error messages.

Code Overview
firstNumber, secondNumber, and result strings: Holds the values of the first and second numbers and the result.
Add, Subtract, Multiply, and Divide functions: Perform the corresponding arithmetic operations.
Clear function: Resets all fields.
ShowError function: Displays error messages.

Exception Handling
Both components use exception handling to validate user input and display error messages. The ShowError function is used to display error messages using the DisplayAlert method of the MainPage of the application. This function takes three string parameters: the title of the alert, the message to be displayed, and the text of the OK button.

When an exception is caught, the ShowError function is called with an appropriate error message. This allows the application to provide a better user experience by displaying meaningful error messages instead of crashing or showing unhandled exceptions.
