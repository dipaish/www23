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