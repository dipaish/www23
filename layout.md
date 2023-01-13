## Buidling a layout for HTML pages

We can use **CSS** to create page layouts and control the position of our html elemets. There are several layout techniques however we will go through some of them

### Normal Flow

You don't do anything for the layout, the normal flow will take the html elements as you have written them in your html code. The elements will be displayed in the **same order** as it appears in the **source code.** The elements that appear one after another are block elements and the ones that appear in the same line are **inline elements.**

**Example of Normal Flow Layout:**
![Normal Layour](assets/images/nlayout.png)

### Flexbox

The flexbox make things easier to put html elemets either in a row or a column. Flexbox is one dimensional that is we can deal with the layout in one dimensiona at a time. We can use flexbox to create flexible and responsive layout.

***To use flex box:***
1.**Flex Container/Elements:** We should first define a **flex container** or specify what **elements** are used as flexible boxes.

```html
display: flex;
```

2. **Columns or Rows:** Flexbox is one dimensional. The property flex-direction specifies which direction the flexbox children are in. By defualt it is set to row.

```html
flex-direction: column;
```

3. **Wrapping:** The equal width and height of flex boxes can result in the child items overflowing their container wich eventually breaks the layout. This can be fixed by adding the following to your flex container.

```html
flex-wrap: wrap;
```

4. **Setting the minimum width for the flexbox children item:**  The following property sets the flexbox children to fit sensibly that is each flex box will be atleast 200px wide.

```html
flex: 200px
```
5. **Flex Box Sizes:**

```html
  article {
    <!-- Equal amount of spaces for items -->
    flex: 1;
    <!-- on adding the folliwing line, third box takes up
    twice as much as the available width of the other two -->
    article:nth-of-type(3) {
      flex: 2;
    }
  }
```

Use ```display:flex``` to the parent html element. All child elements with then become flex items.
```html
    .flexContainer {
        display: flex;
        flex-wrap: wrap;
        background-color: red;
        align-content: space-between;
      }
```
> Unfortunately, Flexbox is not supported in Internet Explorer 10 or earlier versions.

**Example of a flexbox layout:** [Link to the Example file](https://dipaish.github.io/www2020/flexbox.html)

**Let's work together and get the following layouts**
Get HTML code at this link: [Required File](https://dipaish.github.io/www2020/flex_box_in_class22.html)

- [Layout 1](https://dipaish.github.io/www2020/images/Lay1.PNG)
- [Layout 2](https://dipaish.github.io/www2020/images/layout2.PNG)

***Floats***
The float property was introduced to allow web developers to implement simple layouts involving an image floating inside a column of text, with the text wrapping around the left or right of it. The kind of thing you might get in a newspaper layout. Floats are commonly used to create entier website layouts.

**Example of a flexbox layout:** [Link to the Example file ](https://dipaish.github.io/www2020/floatexample.html)

### CSS Grid
A CSS grid is defined using the grid value of the display property; you can define columns and rows on your grid using the grid-template-rows and grid-template-columns properties.

**Some resources for learning CSS grid:**
- https://developer.mozilla.org/en-US/docs/Glossary/Grid
- https://css-tricks.com/snippets/css/complete-guide-grid

## Exercise 4: HTML Layout

- Create a new html page and name it as exercise4.html.
- Write css to create a template as in the image. Use semantic elements such as header, navbar, article, footer in your css. The content and some styles of the page are like you did above.

**Image for the layout**
![Exercise 4: HTML Layout](assets/images/task4.png)

***References***
[MDN Web Docs](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML)

***To learn more***
- https://www.google.fi/search?sourceid=navclient&ie=UTF-8&q=html%2Blearn
- https://www.w3schools.com/html/default.asp