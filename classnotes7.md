# The document object model
## The topmost object in the Document Object Model is the document object.  It represents the web page loaded into the current browser window or tab.
### document.title
* Title of current document
### document.lastModified
* Date on which document was last modified
### document.URL
* Returns string conatining URL of current document
### document.domain
* Returns domain of current document
### document.write()
* Writes text to document
### document.getElementById()
* Returns element, if there is an element with the value of the id attribute that matches
### document.querySelectorAll()
* Returns list of elements that match a CSS selector, which is specified as a parameter
### document.createElement()
* Creates new Element
### document.createTextNode()
* Creates new text node
# EVERYTHING ON PAGES 128 AND 129 ARE SUPER USEFUL

# Data Types
### String
* If a variable, or property of an object, contains a string you can use the properties and methods of the String object on it.
### Number
* If a variable, or property of an object, stores a number, you can use the properties and methods of the Number object on it.
### Boolean
* There is a boolean object. It is rarely used.

## Object

### Arrays are Objects
* An array is a set of key/value pairs but you do not specify the name in the key/value pair of an array - **it is an index number**.

### Functions are Objects
* Technically, functions are also objects.  But they have an additional feature: they are callable, which means you can tell the interpreter when you want to execute the statements that it contains.

## Number Object
* Whenever you have a value that is a number, you can use the methods and properties of the Number object on it.

### isNaN()
* Checks if the value is not a number
### toFixed()
* Rounds to specified number of decimal places
### toPrecision()
* Rounds to total number of places
### toExponential()
* Returns a string representing the number in exponential notation

## Math Object
* The Math object has properties and methods for mathematical constants and functions.

### Math.PI
* Returns pi
### Math.round()
* Rounds number to the nearest integer
### Math.sqrt(n)
* Returns square root of a positive number
### Math.ceil()
* Rounds number up to the nearest integer
### Math.floor()
* Rounds number down to the nearest integer
### Math.random()
* Generates a random number between 0 and 1

# ALL OF PAGES 136 AND 137. CREATING AN INSTANCE OF THE DATE OBJECT

# Creating an Object
## The **new** keyword and the object constructor create a blank object.  You can then add properties and methods to the object.
* First you create a new object using a combination of the **new** keyword and the **Object()** constructor function.
* Once the object is created you can add properties and methods to it using dot notation.  Each statement that adds a property or method should end with a semicolon.
# Creating many objects
## Sometimes you will want several objects to represent similar things.  Object constructors can use a function as a **template** for creating objects.
* **this** keyword is used instead of the object name to indicate the property or method belongs to the object that **this** function creates.
```js
function Hotel(name, rooms, booked) {
    this.name = "new name for hotel"
    this.rooms = "new amount of rooms"
    this.booked = "new amount of rooms booked

    this.checkAvailability = function() {
        return this.rooms - this.booked;
    };
}
```

# Domain Modeling
* Domain modeling is the process of creating a conceptual model in code for a specific problem.

# Tables
```html
<table></table>
```
* The table element is used to create a table.  The contents of the table are written out row by row.
```html
<tr></tr>
```
* You indicate the start of each row using the opening tr tag. **The tr stands for table row**
```html
<td></td>
```
* Each cell of a table is represented using a td element.
```html
<th></th>
```
* The th element is used just like the td element but its purpose is to represent the heading for either a column or a row.

### colspan
* The colspan attribute is used on a th or td element and indicates how many columns that cell should run across.
### rowspan
* The rowspan attribute is used on a th or td element and indicates how many columns that cell should run up and down.

# Long Tables
```html
<thead></thead>
```
* The headings of the table sit inside this element.
```html
<tbody></tbody>
```
* The body should sit inside this element.
```html
<tfoot></tfoot>
```
* The footer belongs inside of this element.