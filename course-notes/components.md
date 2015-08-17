# Components

##HTML Components
Information can be organized in terms of chunks. HTML is a way to organize those chunks in a standard way.

    <!-- HTML Comments are flanked by symbols like this. Comments are essential to helping make any type of programming language readable -->

Essential HTML Components

### Text
```html
    <h1>This is a top level header. You can do h1 down to h6. </h1>
    <h2>Use these to show hierarchies and information groupings</h2>
    <p>This is a paragraph.</p>
    <ol>
        <li>This is an ordered list, where order matters.</li>
        <li>This is a list item. It's marked with numbers.</li>
    </ol>
    <ul>
        <li>This is an unordered list</li>
        <li>Order doesn't matter. It's marked with bullets.</li>
    </ul>
    <!-- This is a comment. It won't show up. on the web page.-->
```

### Media
```html
    <img src="http://wwww.somesite.com/pic.jpg" alt="if picture doesn't exist" title="text on hover">
    <iframe src="someurl"></iframe>
    <video src="someurl" controls> </video>
    <canvas id="someID"></canvas>
```

`img` tags are for images. These are files with formats like `jpg`, `png`, `gif`, or `svg`. 

> Linking to pictures on other sites without permission is a bad practice called 'hotlinking' and should be avoided. Apart from copyright issues, you're using their servers to do your work.

`iframe` tags can pull in anything from videos and audio players to entire other web pages!

> If you want to insert some sort of special content, chances are you can do it with an iframe!

`canvas` tags let you draw things using Javascript. Many powerful charting libraries make use of this.

> Read more about `d3.js` if you're interested in making cool charts!

### Data Collection: Forms
```html
    <form action="someurl.com" method="post">
        <input type="text" name="" id="">
        <input type="email" name="" id="">
    </form>

```

### Secret Sauce of the Internet: Link (Anchor) Tags
```html
    <a href="somewebsite.com" alt="be kind to the blind"> A text link</a>
    <!-- You can also make pictures into links -->
    <a href="somewebsite.com"><img src="coolpic.png"></a>
    <!-- To makea link look like a button, create a class with button styles -->
    <a href="somesite.com" class="button">Submit me</a> 
```
You can make relative links (relative to the page the file is on, which will break if you move the original page) or absolute links (which will work as long as the file you link to doesn't move) 

> Discuss filepath notation if necessary!

There are other worthwhile tags used to help people reading your code understand what's going on.
+ `section`:
+ `nav`: For navigational elements
+ `header` and `footer`
+ `article` 

There is also HTML markup for making tables, drawing canvas
