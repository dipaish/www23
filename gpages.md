# HTML5 & GitHub Pages

## What is HTML5 ?
HTML5 is the most enhanced and latest version of HTML that is used for structuring and presenting content on the World WIde Web. It is a mark up language. HTML5 incorporates features such as drag and drop and video playback which earlier were dependent on third party browser plugins such as Adobe Flash or Microsoft Silverlight

***New features and browser support***
HTML5 has a number of new elements and attribute that can be utilized to build modern web pages. The modern browsers such as Mozilla Firefox, Opera, Google Chrome, and Safari support HTML5. The built in web browsers available in iPhones, iPads and android phones all have support for HTML5. Below is a list of the new HTML5 elements:
- **New Semantic Elements** such as ```<header> <article> <footer>``` for better document structure
- **New Form Elements** such as ```<datalist> <keygen>  <output>```
- **New Input Types** such as ```<color> <email> <url>``` and attributes such as ```<required> <autocomplete> <min and max>```
- **Canvas** HTML5 supports two dimensional drawing surface with the aid of JavaScript.
- **Audio & Video** A video can be easily embedded on web pages without the need of third party plugins.
- **Geolocation** It allows uses to share their physical location with web applications.
- **Drag & Drop** It allows adding drag and drop feature into web pages.

## Semantic Elements in HTML
Semantics describes the meaning of a piece of code in a human and machine-readable way. By just looking into the code you can easily know the purpose and role of the HTML element.

Elements such as ```<header>, <footer> and <article>``` are **semantic** because they accurately describe the purpose of the element and also the content of the element. **Semantic elements** enhance the readability and accessibility of the HTML code whereas **non semantic elements** such as ```<div> <span>``` doest not describe any thing about the content.

### List of Semantic Elements in HTML5

|**HTML Tag**| **Meaning of the Tag**| 
|----------|-------------|
|``` <article>``` |  An article | 
| ```<aside>``` |  Content aside from the page content | 
| ```<details>``` |  Additional details that can be viewed or hidden by user | 
| ```<figcaption>``` |  A caption for a ```<figure>``` element | 
| ```<figure>``` |  Content such as illustrations, diagrams... | 
| ```<footer>``` |  A footer for a document or section | 
| ```<header>``` |  A header for a document or section | 
| ```<main>``` | The main content of a document | 
| ```<mark>``` |  Marked/highlighted text | 
| ```<nav>``` |  Navigation links | 
| ```<section>``` |  A section in a document | 
| ```<summary>``` |  A visible heading for a ```<details>``` element | 
| ```<time>``` |  Date/time | 

***[HTML Element Reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)***

***HTML5 Code Example with Semantic Elements***

```html 
<!DOCTYPE html>
    <html lang="en">
        <head>
            <meta charset="UTF-8">
            <meta http-equiv="X-UA-Compatible" content="IE=edge">
            <meta name="viewport" content="width=device-width, initial-scale=1.0">
            <title>Document</title>
        </head>
        <body>
            <header>
                <nav>
                    <ul> 
                        <li class="nav-links"> <a href="">Home</a> </li> 
                        <li class="nav-links"> <a href="">About Us</a> </li> 
                    </ul> 
                </nav> 
                </header> 
                <main> 
                    <h1>Here is a heading</h1> 
                        <section> <p>hello world</p> </section> 
                </main> 
                <footer> 
                    <p>This is the footer</p> 
                </footer>  
        </body>
    </html> 
```
***HTML Code Example without Semantic Elements***
 ```html
    <html>
        <head>
                <title>Document</title>
            </head>
            <body>
                <div class="header">
                     <div class="nav"> 
                         <ul id="nav-items"> 
                             <li class="nav-links"> <a href="">Home</a> </li>
                              <li class="nav-links"> <a href="">About Us</a> </li> 
                            </ul>
                    </div> 
                </div> 
                <div class="main"> 
                    <h1>Here is the new heading </h1> 
                </div> 
                <div class="content"> 
                    <!-- your content --> 
                </div> 
                <div class="footer"> 
                    <!-- your footer -->
                 </div> 
            </body>
            </html> 
```

## HTML5 Boilerplate
Boilerplate code (boilerplate) are sections of code that are repeated in multiple places with very little to no variation.

In HTML, a boilerplate is the topmost part of the HTML document that is added when you start to create HTML pages. The boilerplate is added to all of your HTML pages.

In **Visual Studio code**, you can get the initial part (boilerplate) of the HTML document by typing **html:5 or !**

```html
 <!DOCTYPE html> 
    <html lang="en">
      <head>
          <meta charset="UTF-8">
          <meta http-equiv="X-UA-Compatible" content="IE=edge">
          <meta name="viewport" content="width=device-width, initial-scale=1.0">
          <title>Document</title>
      </head>
      <body>
         
      </body>
    </html>
```
***Let's look into each of those line***

```<!DOCTYPE html>```
This is the declaration to tell the browser what type of document to expect. You must start your HTML pages with a <!DOCTYPE> declaration.Your HTML pages will work fine even without the declaration however some of the HTML5 tags such as an article or a footer may not be supported by the browser.

```<html lang="en">```
Lang attribute inside the HTML tag sets the language of the webpage. It enhances accessibility that is the screen reader will know the language and will pronounce the text correctly.

```<head> ….. </head>```
Anything that is enclosed in the head tag is not visible in the browser but includes valuable information such as the metadata which describes the document to the machine. It contains information such as the page <title>, links to CSS and other metadata.

```<meta charset="utf-8">```
It specifies the document's character encoding. utf-8 is a universal character set that includes most of the characters from any human language. To display your characters properly (Ä, ö, Å), it is a good idea to include the charset in all HTML pages.

```<meta http-equiv="X-UA-Compatible" content="IE=edge">```
X-UA-Compatible tells the document what version of Internet Explorer the HTML page should be rendered as. The Modern IE browsers are much more compliant with the web standard and therefore there is no need of writing a separate CSS file for the IE browsers which used to be a headache a few years back for website developers.

```<meta name="viewport" content="width=device-width, initial-scale=1.0">```
The viewport is the end user’s visible area of a web page which is different for different devices. The visible area on a mobile phone is smaller than on a computer screen therefore it is required to control the web page’s dimensions and scaling. The width=device-width takes into account the screen width of the device from which a user is viewing the web page while the initial-scale=1.0 sets the initial zoom level for the web page.

### Creating your own HTML5 page
1. HTML5 code should begin with specifying the **DOCTYPE**
2. The character encoding can be specified by using the meta tag
> In Visual studio code, you can get the initial part of the html document by typing **html:5 or !**

```html
    <!DOCTYPE html>
        <html lang="en">
            <head>
                <meta charset="UTF-8">
                <meta name="viewport" content="width=device-width, initial-scale=1.0">
                <title>Document</title>
            </head>
            <body>
                    
            </body>
        </html>
```                
3. Save the file with extension .html for example index.html
> Note: Web browsers ignore spaces and carriage returns in your html code

### Naming HTML Files
- Select names that meaningfully describes the file's contents such as contactus.html, about.html.
- Avoid spaces in your filenames as browsers replace spaces in your filename with characters %20 that can confuse users

## GitHub Pages

***[Quickstart for GitHub Pages](https://docs.github.com/en/pages/quickstart)***

## Exercise 2
Now, let's roll up our sleeves and put our knowledge into action. Head over to this [link](https://gist.github.com/dipaish/a2c1d846c79e518981e19271b9efa828#file-exercise2-md) and follow the instructions in the document to complete the assigned tasks. 


## Common Semantic Elements

1. **`<header>`:**
   - Use this tag to define the header of a document or section.
   - Example:
     ```html
     <header>
         <h1>Page Title</h1>
         <p>Subtitle or tagline goes here</p>
     </header>
     ```

2. **`<nav>`:**
   - Use `<nav>` to define navigation links.
   - Example:
     ```html
     <nav>
         <ul>
             <li><a href="#home">Home</a></li>
             <li><a href="#about">About</a></li>
             <li><a href="#contact">Contact</a></li>
         </ul>
     </nav>
     ```

3. **`<main>`:**
   - Wrap the main content of your page with the `<main>` tag.
   - Example:
     ```html
     <main>
         <!-- Your main content goes here -->
     </main>
     ```

4. **`<article>`:**
   - Use `<article>` to define a piece of content.
   - Example:
     ```html
     <article>
         <h2>Article Title</h2>
         <p>Article content...</p>
     </article>
     ```

5. **`<section>`:**
   - Use `<section>` to define sections in a document.
   - Example:
     ```html
     <section>
         <h2>Section Title</h2>
         <p>Section content...</p>
     </section>
     ```

6. **`<aside>`:**
   - Use `<aside>`for content related to but not directly part of the main content.
   - Example:
     ```html
     <aside>
         <h3>Related Links</h3>
         <ul>
             <li><a href="#link1">Link 1</a></li>
             <li><a href="#link2">Link 2</a></li>
         </ul>
     </aside>
     ```

7. **`<footer>`:**
   - Define the footer of a document or section using `<footer>`.
   - Example:
     ```html
     <footer>
         <p>&copy; 2023 Your Website</p>
     </footer>
     ```
