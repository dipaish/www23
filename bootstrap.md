## What is Bootstrap?
"Bootstrap is an open source toolkit for developing with HTML, CSS, and JS. Quickly prototype your ideas or build your entire app with our Sass variables and mixins, responsive grid system, extensive prebuilt components, and powerful plugins built on jQuery."

**It is responsive and mobile first front-end web development framework.**

**Bootstrap Pages: [Bootstrap](https://getbootstrap.com/)**

***With Bootstrap, you can:***

- Easily create responsive and mobile friendly websites
- Easily create multi-column layout
- Easily create navigation bars and many more other intersting features like image slide, components,tooltips with Bootstrap.

## Getting Started with Bootstrap

To create a bootstrap powered web pages, we first need to integrate it into our environment. There are two methods of adding Bootstrap to your web project.

### Load it remotely
You can add Bootstrap into your project via Content Delivery Network (CDN). It offers performance benefits as they are hosted on multiple servers across the globe, it reduces the loading time.

**Follow the steps below to load Bootstrap:**

1. **Load CSS:To load css, copy-paste the following**

```html

<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta1/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-giJF6kkoqNQ00vy+HMDP7azOuL0xtbfIcaT9wjKHr8RbDVddVHyTfAAsrekwKmP1" crossorigin="anonymous">

```
                        
2. **Load JS:** As several components (jQuery, Popper.js) in bootstrap requires JavaScript to function, it is required to place the following ```<script>``` at the end of your pages before closing the ```<body>``` tag. **jQuery must come first, then Popper.js, and then JavaScript plugins.**

```html

<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta1/dist/js/bootstrap.bundle.min.js" integrity="sha384-ygbV9kiqUc6oa4msXn9868pTtWMgiQaeYH7/t7LECLbyPA2x65Kgf80OJFdroafW" crossorigin="anonymous"></script>

 ```                   
***After doing the above tasks, you can now start to build your webpage using bootstrap***

### Load it locally:

***To install it locally, please follow instructions available at this link:*** [Get Bootstrap](https://getbootstrap.com/docs/5.0/getting-started/download/)

Lets start to build a webpage using Bootstrap

Link to the file: [Link](https://dipaish.github.io/www2020/bootstrap_page.html)
Bootstrap Cheatsheet:[Link](https://devhints.io/bootstrap)

**Example Page with Bootstrap**

 ```html

      <!DOCTYPE html>
      <html lang="en">
      <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Bootstrap - Page Example</title>
        <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta1/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-giJF6kkoqNQ00vy+HMDP7azOuL0xtbfIcaT9wjKHr8RbDVddVHyTfAAsrekwKmP1" crossorigin="anonymous">
      </head>
      <body>
        <h1>Hello, world!</h1>
      
        <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.5.4/dist/umd/popper.min.js" integrity="sha384-q2kxQ16AaE6UbzuKqyBE9/u/KzioAlnx2maXQHiDX9d4/zp8Ok3f+M7DPm+Ib6IU" crossorigin="anonymous"></script>
        <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta1/dist/js/bootstrap.min.js" integrity="sha384-pQQkAEnwaBkjpqZ8RU1fF1AKtTcHJwFl3pblpTlHXybJjHpMYo79HY3hIi4NKxyj" crossorigin="anonymous"></script>
      </body>
      </html>
```   
## Including a Custom CSS

To change the default styling, you don't have to update the css file for bootstrap, you can instead create a child theme and add your own CSS file.

**To add your own css create a file called main.css and link it in the head section of your Bootstrap site.**

 ```html
      <link rel="stylesheet" type="text/css" href="main.css">
 ```
    
## Exercise 5: Building your website with Bootstrap

After going through the above stepts, it is now time a build a website with Bootstrap.

**You are required to include the following items in your website:**
- A navigation bar
- Custom CSS
- Page Content
- A contact us form
- A table
- A footer