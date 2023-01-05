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
- **Geolocation** It alows uses to share their physical location with web applications.
- **Drag & Drop** It allows adding drag and drop feature into web pages.

## Semantic Elemets in HTML
Semantics describes the meaning of a piece of code in a human and machine-readable way. By just looking into the code you can easily know the purpose and role of the HTML element.

Elements such as ```<header>, <footer> and <article>``` are **semantic** because they accurately describe the purpose of the element and also the content of the element. **Semantic elements** enhance the readability and accessibility of the HTML code whereas **non semantic elemenets** such as ```<div> <span>``` doest not describe any thing about the content.

***List of Semantic Elemets in HTML5***

|**HTML Tag**| **Meaning of the Tag**| 
|----------|-------------|
| <article> |  An article | 
| <article> |  An article | 
| <article> |  An article | 
| <article> |  An article | 
| <article> |  An article | 
| <article> |  An article | 
| <article> |  An article | 
| <article> |  An article | 
| <article> |  An article | 
| <article> |  An article | 
| <article> |  An article | 
| <article> |  An article | 
| <article> |  An article | 

***[HTML Element Reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)***

***HTML Code Example with and without Semantic Elements***
| **HTML5 - Semantic Elements **| **HTML - Without Semantic Elements**| 
| ------------- | ------------- |
|``` <!DOCTYPE html>
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
            </html> ```  |  
            ``` <html>
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
             | 