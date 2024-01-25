# What's CSS?

***CSS stands for Cascading Style Sheets.*** It is a style sheet language used to describe the presentation of a document written in HTML or XML (including XML dialects like SVG or XHTML). CSS describes how elements should be rendered on screen, on paper, in speech, or on other media.
***CSS*** separates the structure and content of a document from its presentation, allowing web developers to create visually appealing and responsive web pages. By using CSS, you can define styles for various elements such as fonts, colors, spacing, layout, and positioning.

***Key features of CSS include:***

+ ***Selectors:*** Determine which elements in an HTML document the styles should be applied to.

+ ***Properties:*** Define the visual presentation of selected elements, such as color, size, and positioning.

+ ***Values:*** Specify the particular settings for the properties.

***CSS*** is a crucial part of web development, enabling the creation of consistent and visually pleasing user interfaces across different devices and screen sizes. It also facilitates the maintenance and updating of the design, as changes to the style can be applied globally by modifying the CSS rules, without altering the underlying HTML structure.


## What's CSS used for?

***CSS (Cascading Style Sheets)*** is used for styling and formatting web documents. Its main purpose is to describe how HTML elements should be displayed on a webpage.

***Here are some of the key uses of CSS in web development:***

+ ***Presentation:*** CSS is primarily used to control the visual presentation of HTML elements. It allows web developers to define styles for text, fonts, colors, spacing, backgrounds, and other visual aspects.

+ ***Layout:*** CSS is crucial for creating the layout of a webpage. It enables developers to control the positioning and sizing of elements, including the arrangement of content in columns, grids, or other desired structures.

+ ***Responsive Design:*** CSS is essential for creating responsive web designs that adapt to different screen sizes and devices. Media queries in CSS allow developers to apply different styles based on the characteristics of the device, such as width, height, and resolution.

+ ***Consistency:*** By using CSS, developers can ensure a consistent look and feel across multiple pages of a website. Changes to the styling can be made in one central stylesheet, affecting all pages that reference it.

+ ***Ease of Maintenance:*** Separating the content (HTML) from the presentation (CSS) makes it easier to update and maintain websites. Changes to the visual style can be made without altering the underlying HTML structure.

+ ***Print Styling:*** CSS can be used to define styles specifically for print, allowing developers to create printer-friendly versions of web pages.

+ ***Animation and Effects:*** CSS includes features for creating animations and transition effects without the need for additional scripting languages. This enhances the interactivity and user experience of a webpage.

+ ***Accessibility:*** CSS can be used to improve the accessibility of web content by providing styles that enhance readability and usability for people with disabilities.


## CSS Syntax

***CSS syntax (Cascading Style Sheets syntax)*** consists of a set of rules that define how styles are applied to HTML or XML documents. The basic structure of a CSS rule includes a selector and a declaration block, which contains one or more property-value pairs. 

selector {
    property1: value1;
    property2: value2;
    /* Additional properties and values */
}

##  What's a CSS Selector

+ ***Selector:*** A CSS selector is a pattern used to select and style one or more HTML elements within a document. Selectors define the target elements to which a set of CSS rules or styles will be applied. CSS selectors can be based on various criteria, such as element type, class, ID, attributes, and more.

***Here are some common types of CSS selectors:***

+ ***Element Selector:***

p {
    /* Styles for all <p> elements */
}

+ ***Class Selector:***

.myclass {
    /* Styles for all elements with class="myclass" */
}

+ ***ID Selector:***

#myid {
    /* Styles for the element with id="myid" */
}

+ ***Descendant Selector:***

div p {
    /* Styles for all ```<p>``` elements that are descendants of ```<div>``` elements */
}

+ ***Child Selector:***

div > p {
    /* Styles for all <p> elements that are direct children of <div> elements */
}

+ ***Attribute Selector:***

input[type="text"] {
    /* Styles for all ```<input>``` elements with type="text" */
}

+ ***Pseudo-class Selector:***

a:hover {
    /* Styles for the <a> element when hovered over */
}

+ ***Pseudo-element Selector:***

p::first-line {
    /* Styles for the first line of each <p> element */
}

+ ***Declaration Block:*** The declaration block is enclosed in curly braces {} and contains one or more property-value pairs, each separated by a semicolon ;.

+ ***Property:*** A property is an aspect of the selected element that you want to style, such as color, font-size, or margin.

+ ***Value:*** The value is the setting you apply to the property, such as red for color or 16px for font size.

***Here's an example with a specific rule:***

/* This is a comment */
body {
    font-family: Arial, sans-serif;
    background-color: #f0f0f0;
    color: #333;
    margin: 0;
    padding: 0;
}

***In this example:***

The selector is body.
The declaration block is enclosed in curly braces.
Inside the declaration block, there are several property-value pairs, each ending with a semicolon.
CSS rules are typically written in an external stylesheet file or embedded within the HTML document using the ```<style>``` element in the document's ```<head>``` They can also be applied inline directly to specific HTML elements using the style attribute.


## What are CSS Properties?

***CSS properties*** are settings that define how HTML elements should be displayed on a web page. Each CSS property corresponds to a specific aspect or characteristic of an element, such as its color, size, font, margin, padding, and more. 


***Color Properties:***

+ ***color:*** Sets the text color.

+ ***background-color:*** Sets the background color.


***Typography Properties:***

+ ***font-family:*** Specifies the font of the text.

+ ***font-size:*** Sets the size of the text.

+ ***font-weight:*** Defines the thickness of the characters.

+ ***line-height:*** Sets the height of a line of text.


***Layout Properties:***

+ ***width, height:*** Specifies the width and height of an element.

+ ***margin:*** Sets the margin space around an element.

+ ***padding:*** Defines the padding space inside an element.

+ ***border:*** Sets the border properties (width, style, color).

+ ***display:*** Defines how an element is displayed (e.g., block, inline).


***Positioning Properties:***

+ ***position:*** Specifies the positioning method (e.g., relative, absolute).

+ ***top, right, bottom, left:*** Sets the positioning of an element.


***Text Properties:***

+ ***text-align:*** Aligns the text horizontally.

+ ***text-decoration:*** Adds decoration to the text (e.g., underline).

+ ***text-transform:*** Controls the capitalization of the text.


***Flexbox Properties:***

+ ***display: flex:*** Enables the Flexbox layout model.

+ ***flex-direction:*** Defines the direction of the flex container (row, column).

+ ***justify-content:*** Aligns items along the main axis.


***Grid Properties:***

+ ***display: grid:*** Enables the CSS Grid layout model.

+ ***grid-template-columns, grid-template-rows:*** Defines the grid structure.


***Animation and Transition Properties:***

+ ***animation:*** Specifies the animation properties.

+ ***transition:*** Sets the transition properties for smooth animations.


## How to add CSS (three ways to insert CSS) -> External CSS, Internal CSS, Inline CSS

***External CSS:***

+ Usage:

Best for applying styles consistently across multiple pages.
Enhances maintainability by separating HTML content from styles.
Steps:

Create a separate CSS file with a .css extension (e.g., styles.css).
Link the CSS file to the HTML document using the ```<link>``` tag within the document's ```<head>``` section.

```<!DOCTYPE html>```
```<html>```
```<head>```
    ```<link rel="stylesheet" type="text/css" href="styles.css">```
```</head>```
```<body>```
    ```<!-- HTML content here -->```
```</body>```
```</html>```

***Internal CSS:***

+ Usage:

Suitable for small projects where styles are specific to a single page.
Useful when you want to override external styles for a particular page.
Steps:

Include the ```<style>``` tag within the HTML document's ```<head>``` section.
Write the CSS rules inside the ```<style>``` tag.

```<!DOCTYPE html>```
```<html>```
```<head>```
    ```<style>```
        ```/* Internal CSS rules go here */```
        body {
            background-color: #f0f0f0;
        }
    ```</style>```
```</head>```
```<body>```
    ```<!-- HTML content here -->```
```</body>```
```</html>```


There are three main ways to insert CSS (Cascading Style Sheets) into an HTML document: External CSS, Internal CSS, and Inline CSS. Each method has its own use cases, and the choice often depends on the specific requirements of the project.


***Inline CSS:***

+ Usage:

Used for applying styles to a specific HTML element.
Useful for making quick style adjustments or applying unique styles to individual elements.
Steps:

Apply the style attribute directly to the HTML element.
Write the CSS rules directly within the style attribute.

```<!DOCTYPE html>```
```<html>```
```<head>```
    ```<!-- No external or internal CSS in the head -->```
```</head>```
```<body>```
    ```<p style="color: blue; font-size: 16px;">This is a blue paragraph with a font size of 16px.</p>```
    ```<!-- More HTML content here -->```
```</body>```
```</html>```






