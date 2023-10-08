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
Semantic HTML is basically a **coding style**. It enforces the idea to use the HTML markup 
to enforce the meaning of the element. <br>
Eg. We can use ``<div>`` to define a navigation bar but we should be using ```<nav>``` to enforce
the semantic meaning. <br>
Other examples include - to use ```<strong>``` and ``` <em>``` instead of ```<b>``` and ```<i>``` tags
for bold and italics. <br>
Some semantic elements include : <br>
```<header>``` : defines the header for the document or a section<br>
```<nav>``` : defines a navbar<br>
```<section>``` : defines a specific section of the document<br>
```<article>``` : defines a self-contained section or article<br>
```<aside>``` : content other than normal flow like a sidebar<br>
```<footer>``` : defines the footer of a document <br>


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