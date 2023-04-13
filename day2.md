> # CSS BASICS.
* CSS stands for __Cascading Style Sheets__.
* CSS is used to define styles for your web pages, including the design, layout and variations in display for different devices and screen sizes.

* We use  `<style>` elements at the head section to write the CSS code.

____________________
> ## CSS SYNTAX.

![CSS SYNTAX(](https://www.tutorialstonight.com/assets/css/css-syntax.png)

* __The selector here points to the HTML element you want to style.__

* __The declaration block (All the elements present in between the curly braces) contains one or more declarations separated by semicolons.__

* __Each declaration includes a CSS property name and a value, separated by a colon.__

* Multiple CSS declarations are separated with __semicolons__, and declaration blocks are surrounded by __curly braces__.

> * p is a selector in CSS ( it points to the HTML element you want to style: `<p>`).
> * color is a property, and red is the     property value.
> * margin is a property, and 10px is the property value.
_________

> ## CSS Selectors.

* CSS selectors are used to "find" (or select) the HTML elements you want to style.

> We can divide CSS selectors into __five__ categories:

1. ###  __CSS Element Selector__
The element selector selects the HTML element by name.

> ![](https://www.wikitechy.com/css/img/css-images/code-explanation-css-element-selector.png)

_________________

2. ### __CSS Id Selector__
The id selector selects the id attribute of an HTML element to select a specific element. An id is always unique within the page so it is chosen to select a single, unique element.

* It is written with the hash character (#), followed by the id of the element.

>  `<!DOCTYPE html>`  <br>
`<html> ` <br>
`<head> ` <br>
`<style>  `<br>
`#para1 { ` <br>
    `text-align: center;`  <br>
    `color: blue;  `<br>
`}  `<br>
`</style>  `<br>
`</head>  `<br>
`<body>  `<br>
`<p id="para1">Hello</p>`  <br>
`<p>This paragraph will not be affected.</p>  `<br>
`</body>  `<br>
`</html> `   
___________________
3. ### __CSS Class Selector__
The class selector selects HTML elements with a specific class attribute. It is used with a period character . (full stop symbol) followed by the class name.

> Note __:__ A class name should not be started with a number.

> `<!DOCTYPE html> ` <br>
`<html>  `<br>
`<head>  `<br>
`<style>  `<br>
`.center { ` <br>
 `   text-align: center;  `<br>
 `  color: blue;  `<br>
`}  `<br>
`</style> ` <br>
`</head>  `<br>
`<body>  `<br>
`<h1 class="center">This heading is blue and center-aligned. </h1>`  <br>
`<p class="center">This paragraph is blue and center-aligned.</p>   `<br>
`</body>  `<br>
`</html> ` <br>

________________________________

4. ### __CSS Universal Selector__
The universal selector is used as a wildcard character. It selects all the elements on the pages.

> `<!DOCTYPE html>  `<br>
`<html>  `<br>
`<head>  `<br>
`<style>  `<br>
`p.center {`  <br>
 `   text-align: center;  `<br>
  `  color: blue;  `<br>
`}  `<br>
`</style>`  <br>
`</head>  `<br>
`<body>  `<br>
`<h1 class="center">This heading is not  affected</h1>`  <br>
`<p class="center">This paragraph is blue and center-aligned.</p> `  <br>
`</body>  `<br>
`</html> `<br>
__________________

5. ### __CSS Group Selector__
The grouping selector is used to select all the elements with the same style definitions.

Grouping selector is used to minimize the code. Commas are used to separate each selector in grouping.

> `<!DOCTYPE html>  `<br>
`<html>  `<br>
`<head>  `<br>
`<style>  `<br>
`* {  `<br>
  ` color: green;  `<br>
  `font-size: 20px;  `<br>
`}   `<br>
`</style>  `<br>
`</head>  `<br>
`<body>  `<br>
`<h2>This is heading</h2>  `<br>
`<p>This style will be applied on every paragraph.</p>  `<br>
`<p id="para1">Me too!</p>  `<br>
`<p>And me!</p>  `<br>
`</body>  `<br>
`</html>`    <br>
_______________

> ## CSS PROPERTIES

1. #### background-color: red;
* Sets the background color.Common values assigned to it are:
1. Color name : red, white, black,...
_____________
2. rgb value : rgb(0, 0, 0);
   __Here rgb represents the value of red, green and blue__


       EX: rgb(0,0,0) ; => black.
           rgb(255, 255, 255) ; ==> white.
 _____________________________          
3.  Hex value : It is another way to write RGB. 
 In CSS, a color can be specified using a hexadecimal value in the form:

  >  ## `#rrggbb`

   > Where rr (red), gg (green) and bb (blue) are hexadecimal values between 00 and ff (same as decimal 0-255).

  > For example, #ff0000 is displayed as red, because red is set to its highest value (ff) and the others are set to the lowest value (00).


>  **To display black, set all values to 00, like this:  #000000**.
  **To display white, set all values to ff, like this: #ffffff**.  
_________________
4. RGBA value: rgba(0, 0, 0, 0)
   &nbsp;
   **Here r=red, g=green, b=blue, a=opacity of the color**.
  It can take a value from 0.0 - 1.0. The lower value, the more transparent:
___________________
2. #### color: black;
* Sets the text color. It will also takes the same value as background-color(color name, rgb,hex).
___________________
3. #### height: 35px;
* Sets the height. Common values:
1. pixel value: 36px
2. percentage : 50%
____________
4. #### width: 35px;
* Sets the width. Common values:
1. pixel value: 36px
2. percentage : 50%
________________
5. #### border: none;
* Removes the border.
__________
6. #### border-radius: 2px;
* It creates the round corners.
________________
7. #### border-color: red;
* It sets the border color.
_____
8. #### border-style: solid, dottes, dashed... ;
* dotted - Defines a dotted border
* dashed - Defines a dashed border
* solid - Defines a solid border
* double - Defines a double border
* groove - Defines a 3D grooved border. The effect depends on the border-color value
* ridge - Defines a 3D ridged border. The effect depends on the border-color value
* inset - Defines a 3D inset border. The effect depends on the border-color value
* outset - Defines a 3D outset border. The effect depends on the border-color value
* none - Defines no border
* hidden - Defines a hidden border
________
9. #### border-width: 1px;
* Sets the border-width.
____________
10. #### cursor: pointer;
* Changes the mouse/cursor when hovering over the elements.
____
11.  #### background-image: url("paper1.gif");
* The background-image property is used to set an image as a background of an element.
_______
12. #### background-repeat: repeat-x;  
* By default, the background-image property repeats the background image horizontally and vertically. Some images are repeated only horizontally or vertically.

* The background looks better if the image repeated horizontally only.
background-repeat: repeat-x;
______________
13. ####  Margins
* The CSS margin properties are used to create space around elements, outside of any defined borders.
CSS has properties for specifying the margin for each side of an element:

> margin-top: 10px;
margin-right: 10px;
margin-bottom: 10px;
margin-left: 10px;
________
14. #### CSS Padding
* The CSS padding properties are used to generate space around an element's content, inside of any defined borders.
CSS has properties for specifying the padding for each side of an element:

> padding-top
padding-right
padding-bottom
padding-left
__________

* Shorthand for the 3 properties above.
border: width style color;
border: 1px solid red;
________
> ## HOVER, TRANSITION AND SHADOWS.

> ### HOVER.
* The :hover selector is for selecting the elements when we move the mouse on them. It is not only limited to the links. We can use it on almost every HTML element.
* hover : These styles only apply when hovering over an element.
* active : These styles only apply when clicking on an element.
&nbsp;

 > The hover feature includes the following effects:

* Change the color of the background and font.
* Modify the opacity of the image.
* Text embedding.
* Create image rollover effects.
* Swapping of images.
____________
> ### TRANSITION.

       transition: property  duration ;
        transition: width 2s;
* CSS transitions provide a way to control animation speed when changing CSS properties. Instead of having property changes take effect immediately, you can cause the changes in a property to take place over a period of time.
____________
> ### SHADOWS.
 **box-shadow: &nbsp; Horizontal-position  &nbsp; vertical-position &nbsp; blur  &nbsp; color.**

  i.e  &nbsp;  box-shadow: 10px  10px  5px  lightblue;

  **box-shadow: 3px 4px 5px rgba(0, 0, 0, 0.15);**

Creates a shadow that's 3px to the right of
the element, 4px to the bottom, with 5px of
blur, and a very faint black color.
____________
> ## CHROME DEV TOOLS.
* Chrome Dev Tools are a suite of web developer tools that come pre-installed in the Chrome browser.
* It enables you to make changes to your code, test it, and inspect it.
* Chrome Dev Tools give developers more control over their web applications and browsers.
 &nbsp;
    **To open the DevTools: right-click > Inspect.**
    &nbsp;
    > ![](https://www.freecodecamp.org/news/content/images/2022/02/Untitled-design--1--2.png)

    &nbsp;

    > ![](https://wd.imgix.net/image/admin/aUviBexUPdpxXvUbSUxS.png?auto=format)

    ____________________