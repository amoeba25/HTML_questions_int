# HTML interview questions! 

---
<br>

## 1. Give a brief overview about HTML tables
HTML table tags can be used to display data in tabular form (row and column). 

``<table>`` : defines the table <br>
``<th>``: defines the header cell <br>
``<tr>`` : defines the row in a table <br>
``<td>`` : defines the cell in a table <br>
``<thead>``: used to group the header content in a table <br>
``<tbody>``: used to group the body content in a table <br>
``<tfooter>``: used to group the footer content in a table <br>
``<rowspan>``: used to specify the number of cells an attribute will span<br>
``<colspan>``: used to specify the number of columns a cell should span.

A table example [table](table.html)


## 2. What is semantic HTML? 
Semantic HTML is basically a **coding style**. It enforces the idea to use the HTML markup to enforce the meaning of the element. This coding style will describe the purpose of the element and the type of content that will be inside it. <br>
The two big reasons to use them - **easier to read** and provides **greater accessibility** as Search enginers and assitive tech are all able to better understand the context and the content of your website, creating a better use experience. <br>
Eg. We can use ``<div>`` to define a navigation bar but we should be using ```<nav>``` to enforce
the semantic meaning. <br>
Other examples include - to use ```<strong>``` and ``` <em>``` instead of ```<b>``` and ```<i>``` tags
for bold and italics. <br>
Some semantic elements include : <br>
```<header>``` : defines the header for the document or a section. Usually foud at the top.<br>
```<hgroup>``` : Used wherever we want a main heading with one or more subheadings. Header element can contain any content but the hgroup can only contain other headers : ```<h1>``` to ```<h6>``` <br>
```<section>``` : defines a specific section of the document<br>
```<article>``` : defines a self-contained section or article. This is similar to section tag, the difference being that an article is supposed to be independet or reuseable while a section, it is a thematic grouping of content. <br>
```<aside>``` : content other than normal flow like a sidebar. An example might be we hover over a word and the definition pops up. <br>
```<nav>``` : defines a navbar. We can have a number of nav elements on the page too. Like for example, a global navigation across the top(```<header>```) and local navigation in a sidebar (```<aisde>```)<br>
```<details>``` : defines the footer of a document <br>
```<footer>``` : defines the footer of a document <br>
```<small>``` : this often appears within a footer or aside element where we can have the copyright or other legal disclaimers or other such fine print.  
```<figure>``` :  used to wrap your image content around it<br>
```<figcaption>``` : used to caption those images <br>
```<main>``` :  specifies where the main content of the page starts<br>
```<mark>``` :  used to specify certain texts which are of more importanc like a paragraph that might be more important or relevant. <br>
```<summary>``` : will describe a summary of the document <br>
```<legend>``` : used to define related fieldset together. Eg a form where we might fill name,age etc might have a legend of "personal information" <br>



## 3. What are image maps 
Image maps are used to create specific clickable areas on an image. Here the ```<map>``` element will define an image map 
and ```<area>``` element can be used to create specific areas to click on 

An image map example [imagemap](imagemap.html)

## 4. What is canvas element in HTML5
The ```<canvas>``` element is a container that is used to draw graphics on the web page, 
using scripting languages like Javascript. Allows for dynamic and scriptable rendering 
of 2D shapes and bitmap images 

An example canvas [canvas](canavs.html)

## 5. How would you optimize the websites to load assets quickly? 
There are a number of ways to optimize faster loading of assets <br>
- **CDN hosting** : A content delivery system is basically a geographically distributed servers that can help reduce the latency. Usually, when a user visits a website, the data from that website's servers have to travel across the internet to reach the user's computers. Thus if a user is located far away from that main server, there will be an increased latency. To solve this, the website content is stored on CDN servers that are located closer to the users that can reach their computers faster. <br>
- **File compression** : Method to reduce the overall size of the asset to help reduce the latency. <br>
- **Minify scripts** : Reducing the overall size of CSS and JS scripts <br> 
- **Lazy loading** : Instead of loading all assets at once, the non-critical assets can be loading on a need to need basis. 

## 6. What are the differences between SVG and Canvas HTML5 element

| SVG | Canvas |
| ----------- | ----------- |
| SVG is vector based (composed of shapes) | Canvas is rastar basec (composed of pixels) |
| SVG works better with larger surfaces | Canvas works better with smaller surfaces |
| SVG can be modified with CSS and Scripts | Canvas can only be modified with scripts |
| SVG is highly scalable | Canvas less scalable |

## 7. How can data be stored with web storage in HTML5? 

Webstorage can help to store basic static data in the local storage of the web browser so that we do not need to fetch the data everytime, from the servers. There is a size limit, based on different browsers. There are 2 types of web storage that can be used to store data locally in HTML5: <br>
- Local storage : This will help to store data that can be retained even if user reopens the browser. 
- Session storage : Used only for one session, so as soon as the browser closes, the data will get deleted
- Cookies : This storage mechanism can be manually set. These are a good option for small amount of data that need to be sent to the server, with each request while the local storage is better suited for larger amount of data that need to be persisted between visits to the website. 
<br>

| property |cookie|local storage|sessionStorage
---|-------|-------------|----------------
initiator| client/server. Server can use Set-Cookie header | Client | Client
expiry | Manually set | Forever | On tab close 
Persistent across browser sessions | Depending on expiration set | Yes | No
Sent to server with every HTTP request | Yes, via cookie header | No | No
Capacity (per domain) | 4kb | 5MB | 5MB
Accessibiiity | Any window | Any window | Same tab


## 8. What is SEO? 

SEO or Search engine optimization is the process to make a website more visible in search results or improving the search rankings. Search engines basically crawl the web, follwing one link to next from page to page and index all the content that is found. Crawlers follow certain rules and if we follow those closely, the site will have the best chance of showing up among the first results, increasing the traffic to the website. There are three main methods to SEO: 

- Technical : Using semantic HTML tags. <br>
- Copywriting : Writing content using the vocabulary for the users. Use text as well as images so that the crawler can understand the subject. <br>
- Popularity : We get the most traffic when other established sites link to our website. <br> 

## 9. Why is it a good idea to put ```<link>``` tags between the ```<head>``` and ```<script>``` just before the body? 

Putting ```<link>``` in the ```<head>``` is basically the proper specification that is used to build an optimized website. So when the page first loads, HTML and CSS are parsed simulataneously. The HTML created the DOM and CSS will create the CSSOM, both needed to create the visuals in a website that allows for quick loading. Thus when we put the link tags in the heads, it will ensure that the stylesheets are loaded and ready to use when the browser is done rendering the page. <br>
This is called **progressive rendering**. It is a metric on which sites are measured, based on their performance scores. Putting the stylesheets are the bottom of the document inhibits this progressive rendering. <br> <br> 

The ```<script>``` tag is used just before the body as the script tag block any HTML parsing while they are being downloaded and executed. This can slow down the display of the webpage. Placing them at the bottom will allow the HTML to be parsed and displayed to the user first. 

## 10. What is progressive rendering? 

Progressive rendering is the technique that is used to improve the performance of a webpage (to improve the perceived load time) and to render content as quickly as possible. Some techniques involved to achieve this: <br>
- Lazy loading of images : images on the page aren't loaded, all at once. JS will is used to load an image when the user scrolls onto that part of the page. <br>
- Priortizing visible content only : including minimum CSS/content or scripts necessary for the page. We can use deferred scripts for this <br>
- Async HTML fragments : involves flushing parts of HTML to the browsers as the page is constructed on the backend

## 11. Why would one use a ```<srcset>``` attribute in the image tag? Explain the process that the browser uses the evaluate that content. 

We use ```<srcset>``` when we want to serve different images to the users, depending on the device display width (basically serving hiring quality images to retina display users). This means serving low res images to lower-end devices to increase the performance and decrease data wastage. <br> 
For example: ```<img srcset="small.jpg 500w, medium.jpg 1000w, large.jpg 2000w" src="..." alt="">``` tells the browser to display the small, medium or large .jpg graphic depending on the client's resolution.