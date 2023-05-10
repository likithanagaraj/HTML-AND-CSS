> ## CSS TEXT STYLES.

* The right font can create a strong identity for your brand. The font adds value to your text. It is also important to choose the correct color and text size for the font.

> ## The CSS font-family Property

* In CSS, we use the font-family property to specify the font of a text.

 Ex: **font-family: "Times New Roman", Times, serif**;
* Loads a font from Google onto the page.
 1) Search "google fonts" in Google. 

 2) Pick the fonts and styles that you like.

 3) Copy the code that Google provides into.
  _____________

 > ## Font Style

* The font-style property is mostly used to specify italic text.

* This property has three values:

1. normal - The text is shown normally
2. italic - The text is shown in italics
3. oblique - The text is "leaning" (oblique is very similar to italic, but less supported)

> ### Ex : font-style: normal/italic/oblique;
________________
> ## Font Weight.

* The font-weight property specifies the weight of a font:
 > #### EX :
 >#### 1.font-weight : normal;
 > #### 2.font-weight : bold;
 ______________
 > ## Font Variant

* The font-variant property specifies whether or not a text should be displayed in a small-caps font.

* In a small-caps font, all lowercase letters are converted to uppercase letters. However, the converted uppercase letters appears in a smaller font size than the original uppercase letters in the text.
> #### EX:
> #### font-variant: normal;
> #### font-variant: small-caps;
_________________________
## Font Size

* The font-size property sets the size of the text.

1. Absolute size:
* Sets the text to a specified size.
* Does not allow a user to change the text size in all browsers (bad for accessibility reasons).
* Absolute size is useful when the physical size of the output is known.

2.Relative size:
* Sets the size relative to surrounding elements.
* Allows a user to change the text size in browsers.

  >#### Ex:
  >#### font-size: 40px; 

 ________________
 ## Google Fonts
  * If you do not want to use any of the standard fonts in HTML, you can use Google Fonts.

  * Google Fonts are free to use, and have more than 1000 fonts to choose from.

   ## How To Use Google Fonts
  * Just add a special style sheet link in the <head> section and then refer to the font in the CSS.
  ### Ex:
  > `<head>`
    `<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Trirong">`
   `<style>`
`body {`
 ` font-family: "Trirong", serif;`
`}`
`</style>`
   `</head>`
____________________
   ## CSS DISPLAY PROPERTY.
  * The display property specifies if/how an element is displayed.
     ### 1.The display: Block-level Elements
    * A block-level element always starts on a new line and takes up the full width available (stretches out to the left and right as far as it can).
    * Every HTML element has a default display value depending on what type of element it is. The default display value for most elements is block or inline.

   >  **Examples of block-level elements:**
    1.`<div>`
    2.`<h1> - <h6>`
    3.`<p>`
    4.`<form>`
    5.`<header>`
    6.`<footer>`
    7.`<section>`

   > **Example**
    span.c {
  display: block;
  width: 100px;
  height: 100px;
  padding: 5px;
  border: 1px solid blue;
  background-color: yellow;
}
_____________________
  ## 2.The display:Inline Elements
* An inline element does not start on a new line and only takes up as much width as necessary.
* This is an inline `<span>` element inside a paragraph.
 &nbsp;
    > **Examples of inline elements:**
1.`<span>`
2.`<a>`
3.`img>`

     > **EXAMPLE:**
  span.b {
  display: inline; /* the default for span */
  width: 100px;
  height: 100px;
  padding: 5px;
  border: 1px solid blue;
  background-color: yellow;
_____________
  ### 3.The display: inline-block Elements   
    * Compared to display: inline, the major difference is that display: inline-block allows to set a width and height on the element.
     * Also, with display: inline-block, the top and bottom margins/paddings are respected, but with display: inline they are not.
    * Compared to display: block, the major difference is that display: inline-block does not add a line-break after the element, so the element can sit next to other elements.
    > **EXAMPLE:**
  span.b {
  display: inline-block;
  width: 100px;
  height: 100px;
  padding: 5px;
  border: 1px solid blue;
  background-color: yellow;
}
 ___________________
   ## Div Elements.

  * The `<div>` tag defines a division or a section in an HTML document.
  * The `<div>` tag is used as a container for HTML elements - which is then styled with CSS or manipulated with JavaScript.
  * The `<div>` tag is easily styled by using the class or id attribute.
  * Any sort of content can be put inside the <div> tag! 

   **Note:** By default, browsers always place a line break before and after the <div> element

  >![](https://linuxhint.com/wp-content/uploads/2022/02/text-description-automatically-generated-3.png)
____________
 ## Nested Layout Technique.
 
 * #### There are 2 types of layout.
     **1.  Vertical Layout.**
     **2.  Horizontal layout.**
  &nbsp;

    ![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQGhIbs0p6huXNcLC-yqRQTouaGoHcQBRiGGj50T9avEFXu9qs9yrEJ98WPFJ9X34kkhuo&usqp=CAU)
      &nbsp;

    **Most designs can be created using:**
        
     * Vertical Layout inside horizontal layout inside vertical layout....
           &nbsp;   &nbsp;   &nbsp;    **OR** 
     * Horizontal Layout inside vertical layout inside horizontal layout....

   ### 1. To create the vertical layouts.    
   1. Use `<div>s` with the display: block.
   2. Use flexbox with flex-direction:column;
   3. Use CSS grid with one column.
   ### 2. To create the horizontal layouts.
   1. Use `<div>s` with the display:inline block.
   2. Use flexbox with flex-direction:row;
   3. Use CSS grid with multiple columns.
_____________
 ## Grid Layout

* The CSS Grid Layout Module offers a grid-based layout system, with rows and columns, making it easier to design web pages without having to use floats and positioning.
### 1.Display Property

* An HTML element becomes a grid container when its display property is set to grid or inline-grid.
### EXAMPLE:
> .grid-container {
  display: grid;
 }
______________
## 2.Grid Columns
* The vertical lines of grid items are called columns.
 ![](https://www.w3schools.com/css/grid_columns.png)
________
## 3.Grid Rows
* The horizontal lines of grid items are called rows.
![](https://www.w3schools.com/css/grid_rows.png)
_________
## 3.Grid Gaps
The spaces between each column/row are called gaps.
![](https://www.w3schools.com/css/grid_gaps.png)
### You can adjust the gap size by using one of the following properties:

**1.column-gap
2.row-gap
3.gap**
______
#### 1.The column-gap property sets the gap between the columns:
**Example**
> .grid-container {
  display: grid;
  column-gap: 50px;
}
____
#### 2.The row-gap property sets the gap between the rows:
**Example**
> .grid-container {
  display: grid;
  row-gap: 50px;
}
________
#### 3.The gap property is a shorthand property for the row-gap and the column-gap properties:
**Example**
> .grid-container {
  display: grid;
  gap: 50px 100px;
}
____
#### 4.The gap property can also be used to set both the row gap and the column gap in one value:
**Example**
> .grid-container {
  display: grid;
  gap: 50px;
}
_________
### 4.Grid Lines
* The lines between columns are called column lines.
* The lines between rows are called row lines.
![](https://www.w3schools.com/css/grid_lines.png)
**Example**
> Place a grid item at column line 1, and let it end on column line 3:
.item1 {
  grid-column-start: 1;
  grid-column-end: 3;
}
_______
## All CSS Grid Properties
* ### Property	Description
### 1. Column-gap
* Specifies the gap between the columns.
### 2. Gap
* A shorthand property for the row-gap and the column-gap properties.
### 3. Grid
* A shorthand property for the grid-template-rows, grid-template-columns, grid-template-areas, grid-auto-rows, grid-auto-columns, and the grid-auto-flow properties.
### 4. Grid-area	
* Either specifies a name for the grid item, or this property is a shorthand property for the grid-row-start, grid-column-start, grid-row-end, and grid-column-end properties.
### 5. Grid-auto-columns
* Specifies a default column size.
### 6. Grid-auto-flow	
* Specifies how auto-placed items are inserted in the grid.
### 7. Grid-auto-rows	
* Specifies a default row size.
### 8. Grid-column
* A shorthand property for the grid-column-start and the grid-column-end properties.
### 9. Grid-column-end	
* Specifies where to end the grid item.
### 10. Grid-column-gap	
* Specifies the size of the gap between columns
### 11. Grid-column-start
* Specifies where to start the grid item.
### 12. Grid-gap
* A shorthand property for the grid-row-gap and grid-column-gap properties.
### 13. Grid-row
* A shorthand property for the grid-row-start and the grid-row-end properties.
### 14. Grid-row-end	
* Specifies where to end the grid item.
### 15. Grid-row-gap	
* Specifies the size of the gap between rows.
### 15. Grid-row-start	
* Specifies where to start the grid item.
### 16. Grid-template	
* A shorthand property for the grid-template-rows, grid-template-columns and grid-areas properties.
### 17. Grid-template-areas	
* Specifies how to display columns and rows, using named grid items.
### 18. Grid-template-columns	
* Specifies the size of the columns, and how many columns in a grid layout.
### 19. Grid-template-rows
* Specifies the size of the rows in a grid layout
### 20. Row-gap	
* Specifies the gap between the grid rows.
