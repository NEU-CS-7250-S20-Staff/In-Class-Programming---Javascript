# In-Class-Programming--JavaScript

This repository is your starting point for the assignment and includes the instructions below.

Link to GitHub pages website: `[insert your hyperlink here]`

__Goal__:   
Edit the files to include the functionality described in [this tutorial on w3resource](https://www.w3resource.com/javascript-exercises/javascript-basic-exercise-10.php).

__Submission instructions__:   
Commit your changes to your local repo and push to the remote GitHub repo.
Submit the URL of your repo to the [activity assignment on Canvas](https://canvas.instructure.com/courses/1711075/assignments/12596438).

__Stretch goal__:   
If you are done with the first goal, try to build a simple calculator with all numbers as buttons and operations as buttons too. [This article](https://medium.com/@ethanryan/lets-make-a-javascript-calculator-a81186cb912f) has some ideas you can use, but consider trying things out yourself. You likely won’t be able to get the full thing working in class but it will help you get a hands on experience of working with HTML, CSS and Javascript.

__Additional information__:   
JavaScript (JS) is a high-level, interpreted programming language for computers. It is often run in web browser applications to create things that work by themselves like a popup message or a live clock or counter. It is based on the ECMAScript (ES) standard, and modern browsers support at least ES5.1 and often ES6. In this activity the different features do not matter. You can see [ES6 feature support in this table](https://kangax.github.io/compat-table/es6/).

In the HTML file there is the line:
```
<input type="button" onClick="multiplyBy()" Value="Multiply" />
```
Thwis states that we have an HTML input field here which is of a button type and the value “Multiply” ends up as the button’s label. It also states that when you click the button,the browser is supposed to call the JavaScript function multiplyBy() which is defined in the corresponding JS file. We should write the action that is expected to occur in this function definition.

Function explanation:
```javascript
function multiplyBy(){
        num1 = document.getElementById("firstNumber").value;
        num2 = document.getElementById("secondNumber").value;
        document.getElementById("result").innerHTML = num1 * num2;
}
```

Function keyword states that “multiplyBy” will be defined as follows. Here, it says grab the value of the element having ID=”firstNumber” and put it into a variable called num1 and ID=”secondNumber” into num2. For more info on how this works see [CSS Selectors on w3schools](https://www.w3schools.com/cssref/css_selectors.asp).

Now, grab the element of the document object model (DOM) on the HTML page with ID=”result” and set its innerHTML property. We will now calculate the value by multiplying num1 * num2 and then put this value into ID=”result” by this statement.
document.getElementById("result").innerHTML = num1 * num2;
Some more examples of using innerHTML can be found [on w3schools](https://www.w3schools.com/jsref/prop_html_innerhtml.asp).

