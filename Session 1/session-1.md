# Session 1

A deep dive to various frontend technology that are widely used in the industries, starting with little history of web development how it emerge to overwhelming SDKs and tools.


>## History
1. Static Content [ 1990 to 1995 ]
2. Dynamic Content [ 1995 to 2002 ] 
3. Dynamic **Content** and Interactive UI [ 2002 to 2007 ]
4. Dynamic ~~`Content`~~ ***Data*** to **UI** [ 2007 to 2020 ]
    *   UI Design - Graphics
    *   **UI Development - Programming** <---*This is what we are going to learn with Angular*
  

![Images](/images/web-history.jpg)

># UI Design  - THE PRESENTATION
```
QUESTION: What tools we have to create cool and beautiful presentation? 
```
1. Photoshop - Layout / Image / Graphics / Concept.
2. HTML - Layout of above photoshop.
3. CSS [ Cascading Style Sheet ] - Look of above photoshop.

**Preprocessor**

1. LESS [ [Leaner Style Sheets](http://lesscss.org/) ] - Javascipt based
2. SASS [ [Syntactically awesome style sheets ](https://sass-lang.com/) - Ruby based ]
3. SCSS [ SASSy CSS ]

```
SCSS / SASS / LESS === Tranforms To ===> CSS
```
>###  CSS EXAMPLE - Two body size with table half of the body size

```CSS
.body { width: 200; } /* Small body*/
.table {  width: 100; } /* Half the table size */

.body-large { width: 400; } /* Double of  Large Body */
.table-large { width: 200; } /* Half of the large body size*/
```

>###  SCSS EXAMPLE - Two body size with table half of the body size

```SCSS
$body: 200;
.body: { width: $body; }            //  Generates .body { width: 200; }
.table: {width: $body / 2; }        // .table {  width: 100; }
.body-large { width: $body * 2; }   // .body-large { width: 400; }
.table-large { width: $body; }      // .table-large { width: 200; }
```
># UI Development - **INTERACTION** With Presentation
```
QUESTION: What tools we have to interact with the presentation? 
```
1. **VBScript** - It's a dead dinosaur from Microsoft. ( **Past** ) 
2. **Javascript** - Our Rockstart which evolved and changed the world. ( **Past**, **Present**, and **Future** )
3. **WebAssembly** - At a distant future.


### SO THAT'S IT? WHAT ABOUT, 
1.  **ANGULAR**
2.   **REACTJS**
3.   **CoffeeScript**
4.   **Vue.js**
5.   **The jQuery** - Revolution
6.   **Backbone.js**
7.   **Ember.js**
8.   **Meteor.js**
9.   **Polymer**
10.  **Mithril**
11.  And thousands of many more like that....

They are all either the **JavaScript Framework**, or **Transpiler** to create the complex JavaScript.


># Javascript Journey 


```css
What is Javascript? Where does it excute.

/* It is a client side script that runs within the internet brwoser.*/
```
```css
So the Browser is the **runtime** for JavaScript?

/*Yes, but not really. Each browser comes with it's Own engine.
i.e. 

1. Chakra -     A dying dinosaur from Microsoft - IE11 has this.
2. Chromium -   A open source and now managed by google.
3. V8  -        From Google that integrate Chromium and WebAssembly runtime.

*/
```

```css
Ok great, So What is nodeJS? 

/* It is is server side environment to run the JavaScript. It also has part of Chromium but without any DOM support. */
```

```css
Javascript is the Object Oriented language, is it true?
/* 
    Just to be clear,
    JavaScript is the Language.
    Object Orientation is the Programming Model.

    And we can use the Object Orientted Programming model with JavaScript.
 */
```

> # Let's Dive into JavaScript. 

> ## Early Days of JavaScript.

## Example 1 - Show a message when button is clicked.

 
**HTML**
```html
<html>
    <input type="button" click="showMessage();" value="Click Me" />
</html>
```
 
**JavaScript**
```javascript
function showMessage() {
    alert('Hello World');
}
```
--------------------------------------

## Example 2 - Change Text Box value to "Thanks" when button is clicked.

 
**HTML**
```html
<html>
    <input type="input" id="inputText" />
    <input type="button" click="changeText();" value="Click Me" />
</html>
```
 
**JavaScript**
```javascript
function changeText() {
    
    var inputControl = document.getElementById("inputText"); // Get DOM Object
    inputControl.value = "Thanks"; // Update DOM Object.
}
```
--------------------------------------

## Example 3 - Add three textbox when button is clicked.

 
**HTML**
```html
<html>
    <input id="button1" type="button" click="addTextBox();" value="New Text Box" />
     
</html>
```
 
**JavaScript**
```javascript
function addTextBox() {

    for(int i=0; i<3; i++>) { 

        var element = document.createElement("input");
        element.name = "input" + i;
        element.id = "input" + i;
        element.appendChild(document.createTextNode(""));
        var page = document.getElementById("btn");
        page.appendChild(element);

    }     
}
```

## Example 4 - Add three textbox when button is clicked and each new textbox should show message when value changed.


**HTML**
```html
<html>
    <input id="button1" type="button" click="addTextBox();" value="New Text Box" />
     
</html>
```
 
**JavaScript**
```javascript
function addTextBox() {

    for(int i=0; i<3; i++>) { 

        var element = document.createElement("input");
        element.name = "input" + i;
        element.id = "input" + i;
        element.appendChild(document.createTextNode(""));
        var page = document.getElementById("btn");
        page.appendChild(element);

        /* Couple more lines of code to assign the event. */
    }     
}
```

> ## Birth of AJAX

We can now only request the data or just a section of the web page. 

> ## jQuery - The first JavaScript open source framework.

It changes everything - First Demonstration of Power of javascript. 