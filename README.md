# homework-list-2.0

Create a to-do list of items that correspond to your homework assignments.

## Objective

In this project, we will be using DOM to modify existing HTML elements.

Difficulty: Beginner

## Prerequisites

-Basic understanding of HTML structures. -Basic understanding of DOM.

## Part 1

Create the following:
* HTML file
* CSS file
* JS file
Link all of your files correctly.

## Part 2: Create a "close" button and append it to each list item

create an array that gets all the elements with tag name "li"
create a for-loop that iterates from var i = 0 to the length of the array

Inside the for-loop:
create a variable called 'span' and store in it a new element with the tag name "span"
ex: var span = document.createElement("span");
create a variable called 'txt' and store in it a new text node of the unicode for the multiplication sign, which looks like "x". The unicode for the multiplication sign is "\u00D7".
set the class name of the span variable equal to "close"
append the txt variable as the child node to span
ex: span.appendChild(txt)
append the span variable as the child node to the array element at index i
ex: arr[i].appendChild(span)


## Part 3: Add “close” button functionality

create an array called 'close' that gets all the elements with class name "close"
ex: var close = document.getElementsByClassName("close")
create a for-loop that iterates from var i = 0 to the length of the close array

Inside the for-loop:
create a function that takes no parameters.

Inside the function:
create a variable called 'div' and set it to "this.parentElement"
set the style.display attribute of the div variable to "none"
ex: variable.style.display = "none"
Close your function!
set the array element at index i to the function, when clicked.
ex: close[i].onclick = functionName()


## Part 4: Copy and paste this code to check off the list item when clicked

var list = document.querySelector('ul');
list.addEventListener('click', function(ev) {
if (ev.target.tagName === 'LI') {
ev.target.classList.toggle('checked');
}
}, false);

## Part 5: Create a new list item when “add” button is clicked

create another function that takes no parameters.

Inside the function:
create a variable called 'li' that creates an element with the tag name "li"
create a variable called 'inputValue' that gets the value of the element with the ID "myInput"
create a variable called 'newText' that creates a text node containing the inputValue variable
append the newText variable as the child to the li variable

Check if the input value is valid by:
Create an if-else statement, which checks if the input value is blank
if the inputValue === '', then write an alert telling the user they must type something.
Else, then input is considered valid. Append the li variable as the child to the element with ID "myUL"

set the value of the element with ID="myInput" to ""
create a variable called 'span' and store in it the new element of the tag name "span"
create a variable called 'txt' and store in it a new text node of the unicode for the multiplication sign, which looks like "x". The unicode for the multiplication sign is "\u00D7".
set the class name of the span variable equal to "close"
append the txt variable as the child node to span
ex: span.appendChild(txt)
append the span variable as the child node to the li variable
ex: li.appendChild(span)

Create the same for-loop from Part 2 using Lines 2-4.
Close your function!

## Part 6: Create the removeAll() function to add functionality to the “Clear Items” button

create a function called 'removeAll' that takes no parameters.
Inside the function:
create an array called 'list' and store in it all the elements with the tag name "ul"
set the list[0].innerHTML to an empty string ""


