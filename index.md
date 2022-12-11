
# Basics of HTML
## What is HTML?
**Hypertext Markup Language (HTML)** is the standard markup language for documents that are designed to be displayed in a web browser. HTML is not a programming language. It is a markup language that tells browser how to structure a web page. HTML is made up of sereis of **elements** such as a piece of text, a pragraph, , list, table, links or forms.

>> Lets write the following line of text in a text file and save it as **file1.html**
I am learning to develop web pages
Now lets use the paragph tag by modifying **file1.html**
<p>I am learning to develop web pages.</p>
>> Note: Tags in HTML are case-insensitive. This means they can be written in uppercase or lowercase. However, it is strongly recommended to write all tags in lowercase for consistency, readability, and other reasons.

A simple HTML document looks like this
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
```html <!DOCTYPE html>```
It is simply meant to act as links to a set of rules tht the HTML page had to follow. In current time, rarerly anyone cares about it however it is recommended to start with the DOCTYPE.

```html<html></html>```
This element simply wraps all the content on the entire page, and is sometimes known as the root element.

```html<head></head>``` 
This element acts as a container for all the stuff (keywords, page description,css, character set declarations and more) you want to include on the HTML page, that isn't the content you are showing to your page's viewers.

```html<title></title>```
his element defines the title of your page, that appears in the browser tab and is used to describe the page when you bookmark/favorite it.

 ```html<body></body>```
This element contains all the content that is displayed to web users such as text, images, videos or games.

### References: 
- 

