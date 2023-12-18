## What is CSS?
CSS (Cascading Style Sheets) is a style sheet language for creating great-looking web pages. It describes the presentation of elements in a document. You define a group of styles that are applied to particular elements on your web page. For example, you want the main heading to be shown as large red text.

### Inline CSS
- It is often used to apply a style for a single html element.
- To add inline CSS, you can simply add the style to the corresponding element.

> Example of Inline CSS

```html
<h1 style="color:brown;text-align:left;">This is my heading</h1> 
<p style="color:red;">This is a paragraph.</p>
``` 
### Embedded CSS
The embedded CSS or the internal CSS is written inside the ```<style>``` element in the ```<head>``` section of your HTML document.

> Example of embedded CSS

```html
      <!DOCTYPE html>
      <html>
      <head>
      <style>
      body {
        background-color:red;
      }
      h1 {
        color: blue;
      }
      </style>
      </head>
      <body>
      <h1>This is a heading</h1>
      <p>This is a paragraph.</p>
      </body>
      </html>
```
### External css
The best way of adding a CSS to your html document is by creating a css file with an extension .css.

**Linking the css**
To link style.css to index.html add one of the following line somewhere inside the <head> of the HTML document.

```html
<link rel="stylesheet" href="style.css">
<link href="css/style.css" rel="stylesheet" type="text/css">
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css">
```
### CSS: Selectors
CSS selector defines what elements should the CSS property be applied.
![HTML Element](assets/images/cssselector.png)


## ID & CLASS

In HTML and CSS, we use both **ID**s (Identifiers) and **classes** to identify and style elements.

**ID**
IDs help you precisely pinpoint HTML elements. They provide a high level of specificity in CSS selectors, which means they have a special way of determining which styles should be followed when there are conflicting rules.

When you apply styles to an ID, those styles take precedence over styles applied to elements with classes or generic element selectors. This unique feature makes IDs particularly powerful for giving a distinct and individual style to specific elements on a webpage. It's like giving them a special treatment that stands out from the rest of the styling.

***Syntax in HTML***
```
<tag id="uniqueId">Content</tag>
```

***Syntax in CSS***
```
#uniqueId {
    /* styles */
}
```

***Example***
```
<div id="header">This is a Header</div>
<style>
#header {
    background-color: #333;
    color: white;
    padding: 10px;
}
</style>
```

**CLASS**

Multiple elements can share the same class. A class can be applied to any number of elements.Classes have lower specificity than IDs. They are useful for styling multiple elements consistently without the need for uniqueness. Classes promote the reuse of styles across different elements or sections of a webpage.

***Syntax in HTML***
```
<tag class="className">Content</tag>
```

***Syntax in CSS***
```
.className {
     /* styles */ 
     
     }
```

***Example***
```
<p class="highlight">This is a highlighted paragraph.</p>
<style>
.highlight {
    background-color: yellow;
    padding: 5px;
}
</style>

```

**CSS Example**
- [Example Page](https://dipaish.github.io/www2020/cssexample.html)
- [CSS File](https://raw.githubusercontent.com/dipaish/www2020/master/docs/css/learncss.css) 

## CSS Validator
To validate your CSS style sheet, you can use the CSS Validation service at this link: [CSS Validation service](https://jigsaw.w3.org/css-validator/)

**To learn more:**
- https://www.google.fi/search?sourceid=navclient&ie=UTF-8&q=html%2Blearn
- https://www.w3schools.com/html/default.asp
- CSS Reference: https://cssreference.io/

## Exercise 4
It is now time to apply what you have learnt, please find the exercise at the link below: 
***[Exercise 4](https://docs.google.com/document/d/1_Jjq6BvFO_p34vSD2S0kGBkt-irFea4L/edit?usp=share_link&ouid=111470325935077300698&rtpof=true&sd=true)***