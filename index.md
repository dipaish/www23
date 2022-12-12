# Basics of HTML
## What is HTML?
**Hypertext Markup Language (HTML)** is the standard markup language for documents that are designed to be displayed in a web browser. HTML is not a programming language. It is a markup language that tells browser how to structure a web page. HTML is made up of sereis of **elements** such as a piece of text, a pragraph, , list, table, links or forms.

***Lets write the following line of text in a text file and save it as*** **file1.html** 

```html
I am learning to develop web pages
```

*** Now lets use the paragraph tag by modifying*** **file1.html**
```html
<p>I am learning to develop web pages.</p>
```

>> Note: Tags in HTML are case-insensitive. This means they can be written in uppercase or lowercase. However, it is strongly recommended to write all tags in lowercase for consistency, readability, and other reasons.

***A simple HTML document looks like this***
```html
    <!DOCTYPE html>
    <html lang="en">
     <head>
      <title>My page</title>
     </head>
     <body>
      <h1>My page</h1>
      <p>This is a <a href="link">simple</a> Link</p>
      <!-- this is a comment -->
     </body>
    </html>
```   

| Tag  | Description |
| ------------------------- | ------------- |
| ``` <!DOCTYPE html> ``` | It is simply meant to act as links to a set of rules tht the HTML page had to follow. In current time, rarerly anyone cares about it however it is recommended to start with the DOCTYPE.  |
| ``` <html>  </html> ```  | This element simply wraps all the content on the entire page, and is sometimes known as the root element.  |
| ``` <head></head> ```  | This element acts as a container for all the stuff (keywords, page description,css, character set declarations and more) you want to include on the HTML page, that isn't the content you are showing to your page's viewers.|
| ``` <title></title> ```   | This element defines the title of your page, that appears in the browser tab and is used to describe the page when you bookmark/favorite it.  |
| ``` <body></body> ``` | This element contains all the content that is displayed to web users such as text, images, videos or games.  |


## HTML Elements
As in the above example, **html** document consists of a **tree** of elements and text. Each element starts with a **tag** and ends with a **tag.** Tags have to be **nested** such that they are completely within each other without **overlapping**.

```html
<p>This <em>is <strong>correct</strong>.</em></p>
<p>This is <em>very <strong>wrong</em>!</strong></p>
```
![HTML Element](assets/images/element.png)
>> Note: Tags in HTML are case-insensitive, i.e. they can be written in uppercase or lowercase. Best practice, however, is to write all tags in lowercase for consistency, readability, and other reasons.

***There are two important categories of elements in HTML.***
- **Block Level Elements:**
Block-level elements form a visible block on a page. A block-level element appears on a new line following the content that precedes it. Any content that follows a block-level element also appears on a new line. Block-level elements are usually structural elements on the page. For example, a block-level element might represent headings, paragraphs, lists, navigation menus, or footers. A block-level element wouldn't be nested inside an inline element, but it might be nested inside another block-level element.
Example:
```html
      <p>paragraph 1</p><p>paragraph 2</p><p>paragraph 3</p><p>paragraph 4</p>
```

- **Inline Elements:**
These elements are contained within the block level elements that is it does not cause a new line to appear in the document.
Example:

```html   
      <em>element 1</em> <em>element 2</em> <em>element 3</em>
```

## Whitespaces in HTML
The whitespace includes space characters as well as line breaks. You can have lots of whitespaces in your code but the HTML parser reduces space(s) or line breaks into a single space when rendering the HTML code. There is no reason to use more white spaces as it might affect the readability if it is not nicely formatted.
```html 
<p> this is properly formatted in terms of whitespaces</p>
    <p>this is 
      very                    random and is not effective enough when 
      reading 
      the 
      code. 
    </p>
```

## Using Special Characters in HTML
** <, > , " and & ** are special characters which are parts of HTML syntax, Therfore, when you need to use them in your html code you need to use the character equivalent as in the table below, to not have it interpreted as code.

| HTML Character  | Equivalent Character Reference |
| ------------- | ------------- |
| < | &lt; |
| >	| &gt; |
| " | &quot;|
| '	|&apos; |
| &	| &amp; |

## Comments in HTML

## Text formatting in HTML

## Images in HTML

### Example 1: Image and Content

### Example 2: Side by Side Images

### Example 3: Stacking Images

## Exercise 1: Text Formatting and page content

## References: 
- Mdn Web Docs 

>> To learn more

