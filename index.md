# Basics of HTML

## Tools for web development
You need atleast some of the following tools to get started with web development. Depending on your development activity (frontend, backed or full stack), you will need some of the following tools. You will need at the minumm code or text editor and a browser.

- **Code or Text editors:** Sublime Text, Notepad++, ***Visual Studio Code***
- **Front-End Frameworks:**  Bootstrap, Semantic-UI, Material UI
- **Web Application Frameworks:**  Django, Angular, ReactJS
- **Package Managers:**  NPM, Yarn, Material UI
- **Git Clients:**  Github, Github Desktop
- **Web Design & Prototyping Tools:**  Figma, Protooie, Framer
- **Image Editing:**  Adobe Photoshop, Gimp
![Development Environment](assets/images/devenvironment.png)


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
| -------------| ------------- |
| ``` <!DOCTYPE html> ```       | It is simply meant to act as links to a set of rules tht the HTML page had to follow. In current time, rarerly anyone cares about it however it is recommended to start with the DOCTYPE.  |
| ``` <html>  </html> ```        | This element simply wraps all the content on the entire page, and is sometimes known as the root element.  |
| ``` <head></head> ```          | This element acts as a container for all the stuff (keywords, page description,css, character set declarations and more) you want to include on the HTML page, that isn't the content you are showing to your page's viewers.|
| ``` <title></title> ```         | This element defines the title of your page, that appears in the browser tab and is used to describe the page when you bookmark/favorite it.  |
| ``` <body></body> ```      | This element contains all the content that is displayed to web users such as text, images, videos or games.  |


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
```<, > , " and &``` are special characters which are parts of HTML syntax, Therfore, when you need to use them in your html code you need to use the character equivalent as in the table below, to not have it interpreted as code.

| HTML Character  | Equivalent Character Reference |
| ------------- | ------------- |
|``` < ```| ``` &lt; ``` |
| ``` > ```	| ``` &gt; ``` |
| ``` " ``` | ``` &quot; ```|
|``` ' ```	|``` &apos; ``` |
|``` & ```	| ``` &amp; ``` |

## Comments in HTML

It is a good idea to write comments whereever applicable. Comments are ignored by the browser and are invisible to the user.
***To type comment in HTML:***
```html 
 <!-- comment asdsad asdasda -->
 ```

## Text formatting in HTML

- HTML is used to structure text within a page by adding headings, paragraphs, emphasizing words and more.

- The structured content provides a better and enjoyable reading experience.

- Headings are to be wrapped in a heading element ```<h1>```. There are 6 level of heading elements ```<h1>, <h2>, <h3>, <h4>,<h5> & <h6>```.

- Paragraphs are wrapped in a ```<p>```

```html 
<h1>My heading</h1>
<p>This is a paragraph.</p>
 ```
***Example of a Structure***
![Example of a strucutre](assets/images/structure1.png)

### Lists: Unordered
```html 
<ul>
<li>Deepak</li>
<li>Markku</li>
<li>Pekka</li>
<li>Juha</li>
</ul>
```

### Lists: Ordered
```html 
<ol>
<li>Deepak</li>
<li>Markku</li>
<li>Pekka</li>
<li>Juha</li>
</ol>
```

### Lists: Nested
```html 
<ol>
<li>Chapter 1</li>
<li>Chapter 2</li>
<li>Chapter 3</li>
<li>Chapter 4
<ul>
<li>Chapter 4.1</li>
<li>Chapter 4.2</li>
</ul>
</li>
</ol>
``` 
### Emphasizing Certain Words

It is sometimes needed to emphasize certain words within your text. HTML provides several semantic elements to mark up textual content with different effects.

**Emphasis:** ``` <em>...</em> ``` This is <em> emphasized text.</em>

**Bold:** ``` <b>...</b> ``` This is <b>bold text.</b>

**Strong:** ``` <strong>...</strong> ``` This is <strong> strong text.</strong>

**Italic:** ``` <i>...</i> ``` This is <i>italicized text </i>.

**Underline:** ``` <u>...</u> ``` This is <u>underlined text.</u>

## Images in HTML

The img element and its src attribute are used to embed an image in HTML.
```html 
<img src="/images/myimage.jpg" alt="" width="100“ height="150"> 
<img src="https://raw.githubusercontent.com/dipaish/www2020/master/docs/images/header.png " width="680px">
<img src="images/missing.jpg" alt="Photo info"/>
<img src="images/missing.jpg" alt="Photo info" height="200px" width="200px"/>
```  
**Image Sizes**
You may use width and height attribute to size image however it is recommended to use photo editing software to determine the size of images to produce a better result. Resizing images properly will download faster when users view your pages.

***Image size can also be specified as a windows percentage.***

```html 
<img src="https://raw.githubusercontent.com/dipaish/www2020/master/docs/images/header.png " alt="Photo info" width="30%"/>
```

**Alternative Text**
The **alt** attribute is a textual description of the image that is displayed to the user when am image is not found or takes a long time to render due to slow internet connection. It is also handy for visually impaired user who is using a screen reader to read the web.

```html 
<img src="images/img1.jpg" alt="info about image">
```

**Image Titles**
The ***title*** attribute in image provides a tooltip on mouse over.It is however not recommended due to various accessibility problems.

```html 
  <img src="images/img1.jpg" alt="info about image" title="more info">
``` 
### Image Captions in HTML5
You can use ```<figure> and <figurecatpion>``` elements.
```html 
    <figure>
      <img src="images/img2.jpg" alt="image 2;">
    <figcaption>Image caption</figcaption>
    </figure>
```
***Understanding Image URLS & Important Notes***
- The **src** attribute in img tag locates the image file
- There are two types of URLs: **Absolute & Relative**
    - **Absolute:** The exact location of the image that normally begings with http://....
    - **Relative:** To better organize, images are stored within a specific folder. In such cases, you can use relative location such as images/image1.jpg
- Search engines also read image filenames and count them towards SEO. Therefore, it is wise to use a descriptive image filename; apple.jpg is better than img135.png.
- Make sure, you own copyrights before displaying an image in your webpage.
- Images garner attention and draw emotion therfore use images wisely as people pay more attention to image than text.
- Try to limit larger size images as much as possible so that they are not slowing down your website.

## Exercise 1: Text Formatting and page content
***Create a (root)folder anywhere in your PC/Cloud and name it as your firstname_lastname*** for your website(all individual exercises). Your website has different types of files: codes (html, css) and assets such as images.

- Create a proper folder structure
- Create an index.html
 
***The page should look as below:***
![Your Index Page for exercises](assets/images/ex1.png)

- Use heading1 for "your name"
- Use heading2 for "List of all Individual Exercises"
- Exercise1 in the list should **link** to the file exercise1.html [Creating hyperlinks](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks)
- Visit any website of your choice. Make an HTML page that has roughly the same content. You don't need to worry about formats, backgrounds or colors. The main objective is to use elements and tags correctly in HTML.You can ignore the menu bar,left or side bars. Follow the guidelines below:

    - Start writing your html code. Save the file as exercise1.html and do all following tasks in the same file
    - The HTML head is the contents of the ```<head>....</head>``` element. The content of the head element is not displayed to the user. It contains metadata about the document such as the author information, the title of the page, the metadata element such as the document's character encoding, custom icon to your page, link to the CSS and JavaScript file that are applied to the pages, primary language of the document, Your task is to include a proper title, the author information,set the character set as utf-8 and a brief description that is used on a search engine result pages.For this task, please consider reading this document: [What's in the head?](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML)
    - The top level heading of the page can be heading 1
    - Put some random text pieces in the  ```<p>``` tag
    - Add a couple of random link to some external pages.
    - Apply some text formatting such as bold, italic, underline to some part of your text.
    - Add an image to your page

## References: 
- Mdn Web Docs 

>> To learn more

