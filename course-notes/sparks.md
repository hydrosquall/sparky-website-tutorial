## Making Modern Websites: Basic Site

We've come a long way since the websites of the 90s! What changed?
> While waiting, checkout these blasts from the [past](http://retrosite.ninja/)!

![Facebook before](http://cnet1.cbsistatic.com/hub/i/r/2014/02/03/f1e9d629-a5c4-11e3-a24e-d4ae52e62bcc/resize/1170x878/5c34b29efda0801143249cc83b048e75/2005_17.jpg)

In other cases...
+ [Greenlight Capital](https://www.greenlightcapital.com/) (Worth $10 Billion)
+ [Berkshire Hathaway](http://www.berkshirehathaway.com/) (Website of Warren Buffett, World's Wealthiest Man)

Adding more elements isn't necessarily the answer. 
![Bad Web Design](http://wpbusinesstips.com/wp-content/uploads/2014/08/baddesign2.jpg)

Every website should be written with a clear goal that keeps the audience in mind! The "grammars" of HTML, CSS, and JS that we learn are small details, don't sweat them. A missing semicolon can be fixed by a robot and/or a trained monkey. On the other hand, thoughtless information design requires a thoughtful person to recover from.

### Page Architecture

Every website has a story to tell. Like a good essay, every page should have an engaging beginning, a clearly organized middle, and an impactful end. It may also include a navigational section to help you look for other pages. The source html for a bare website looks something like this in pseudo-code.

`index.html`
```
    Navigation
    Compelling Beginning Content
    Meaty Middle Content
    Exciting Ending Content
    Page Footer
```

A bare-bones website doesn't have any CSS or JS, because the HTML is the place for raw content. Think about what kind of mini-story you'd like to tell with your website. We're going to make a dummy website for an Idea Factory to help other peoples' ideas come to life! 

### To Build a Fire: HTML Elements

####Part 1: Learn the ABCs: HTML Elements
> Read [components](components.md) and discuss bonus elements

We will be using a combination of `<div>`, `<h1>`, `<p>`, `<ul>`, `<img>`, and `<a>` tags. 

####Part 2: Using Components

This is the foundation of your website. Paste this into `index.html` to begin. We'll talk through each piece step by step. 

You can paste each region below the previous region in the "body" area of your foundation. There is a little bit of hand-waving happening here in the interest of saving time, but leave a comment [here](https://github.com/hydrosquall/sparky-website-tutorial/issues) if you get stuck and I'll try to help!

If you think you have an indentation problem, the [HTML Prettifier](http://www.dirtymarkup.com/) can help you fix your code so it's easier to read.

Feel free to make duplicates of any block, or skip blocks altogether! Doing this is mainly for the muscle memory. Once you understand multiplication, you don't need to keep counting 1 by 1 to convince yourself that it works.
```html
    <!DOCTYPE html>
    <html lang="en">
        <head>
            <meta charset="UTF-8">
            <!-- optional metadata tags -->
            <title>WEBSITE TITLE</title>
            <!-- link to styles -->
        </head>
        <body>
            <!-- Add website body content -->
            <!-- link to scripts -->
        </body>
    </html>
```

**Navigation Bar**
```html
    ... <!-- This is the first block -->
    <div class="hold">
      <div class="header">
        <div class="container">
          <div id="logo"></div>
          <ul class="nav">
            <!-- This is a page link -->
            <li><a href="#">Demo</a></li>
            <!-- Make 3 more links! -->
          </ul>
        </div>
      </div>
    </div>
    ...
```

**Hero Section**
```html
    ...
    <div class="section">
      <div class="slider">
        <div class="container slidercontent">
          <h1 class="hero">Spark!</h1>
          <h2 class="hero">A Modern Idea Factory</h2>
          <div class="call"><a href="https://github.com/hydrosquall/sparky-website-tutorial">Learn More</a></div>
        </div>
      </div>
    </div>
    ...
```

** Pitch Section**
Note we are using emoticons ( `:)` ) instead of pictures to save data! However, you could use icons from font-awesome instead.

```html
    ...
     <div class="section">
      <div class="container">
        <h1 class="callout">Whatever challenges you face, we can help.</h1>
      </div>
    </div>
    <div class="section">
      <div class="container">
        <!-- This is a service-block -->
        <div class="col four">
          <h1 class="icon">[]</h1>
          <h1 class="service">Duct Tape</h1>
          <p>For all your mechanical engineering needs!</p>
        </div>
        <!-- Repeat 3 more service-blocks -->
        <!--<div class="responsivegroup"></div> -->
      </div>
    </div>
    ...
```

**Pictures Thumbnails Area**
```html
    <div class="section bg">
      <div class="container">
        <h1>Projects</h1>
        <h2>We have built cool things in all these places!</h2>
        <!-- this is a place card -->
        <div class="col three bg nopad pointer">
          <div class="imgholder"></div>
          <h1 class="feature">USA</h1>
          <p>Wow wow</p>
        </div>
       <!-- Make 2 more place cards -->
        <div class="group margin"></div>
       <!-- this Make 3 more place cards -->
      </div>
    </div>
```

**Team Bios**
```html
    <div class="section">
      <div class="container">
        <h1>Our Team</h1>
        <h2>Professional and Experienced!</h2>
        <!-- This div holds a team card. -->
        <div class="col three">
          <h1 class="icon side">ಠ_ಠ</h1>
          <h1 class="feature side">Suspicious Bob</h1>
          <p class="side">Bob pays *very* close attention to detail.</p>
        </div>
       <!-- Repeat the team-card item 2 more times -->
        <div class="group margin"></div>
        <!-- Repeat the .col three 3 more times -->
        <div class="group margin"></div>
      </div>
    </div>
```

**Testimonial Cards**
```html
   <div class="section bg">
     <div class="container">
       <h1>Testimonials</h1>
       <h2>Happy Customers or your money back!</h2>
       <!-- This is a testimonial! -->
       <div class="col two bg margin extrapad">
         <h1 class="icon side">A+</h1><span class="feature side">JP</span><span class="side"> - Bird Wrangler</span>
         <p class="side">Don't let the wow drive the bus</p>
       </div>
        <!-- Why not add a few more? -->
     </div>
   </div>
```

**Two Column Layout Call to Action**
```html
    <div class="section">
      <div class="container">
        <!-- This is the first column -->
        <div class="col two">
          <h1 class="icon">work</h1>
          <p>Want to get started? <a href="#">Submit Idea</a></p>
        </div>
        <!-- Why not add a second one? column -->
      </div>
    </div>
```

**Footer**
Feel free to change the text and links!
```html
    <div class="section">
      <div class="footer">
        <div class="container white">
          <div class="col four left">
            <h1>What?</h1>
            <p>This is a basic modern website.</p>
            <p>You can use it to showcase your product or business!</p>
          </div>
          <div class="col four left">
            <h1>How?</h1>
            <p>CSS3 and HTML. JS for header shrinking; optional. Site works perfectly with JS disabled </p>
          </div>
          <div class="col four left">
            <h1>Why?</h1>
            <p>Many popular HTML themes have thousands of lines of HTML, thousands of lines of CSS and several JS plugins on every page amounting to tens of thousands of lines of JavaScript.</p>
            <p>This is a lightweight way to achieve some stylish modern effects!</p>
          </div>
          <div class="col four left">
            <h1>Who?</h1>
            <p>This site was created for a <a href="https://github.com/hydrosquall/sparky-website-tutorial">tutorial </a>by <a href="http://www.cameronyick.us">Cameron Yick. </a></p>
            <p>It is based upon <a href="http://atunnecliffe.com" target="_blank">Andrew Tunnecliffe's</a> 'Every Modern Website'.</p>
          </div>
          <div class="group"></div>
        </div>
      </div>
    </div>
```

You can see a finished copy of the site in the `reference-files` folder or live [here](http://www.cameronyick.us/sparky/)

### Sparkly Sparks: CSS for Styles

So much typing, and yet the site doensn't look so great! What happened?

Let's add this line to the page head:

```html
    <!DOCTYPE html>
    <html lang="en">
        <head>
            <meta charset="UTF-8">
            <title>WEBSITE TITLE</title>
            <link rel="stylesheet" type="text/css" href="assets/styles.css">
        </head>
```
Whoa! The site should look significantly better. How did that happen?

> If you're using the Codepen version of the tutorial, don't worry about this step. The stylesheet (the collection of CSS declarations) was inserted automatically.

![Anatomy of a rule](http://ironion.com/wp-content/uploads/2015/06/cssanatomy1.png)
_The stylesheet is made of a bunch of these!_

#### Part 1: Learn the ABCs: CSS Declarations
+ Breaking Down the Stylesheet + Cascading Effect
+ Selectors: Elements, .Classes, and #IDs
+ Selectors: Chaining Selectors
+ CSS Styles: Google them and learn by doing

> Covered in lecture

The declarations "cascade" (the **C** in CSS) from top to bottom. This means that if multiple declarations affect a property, the last declaration will override the previous ones. Basically when there are conflicts, the last rules wins. 

This means you should make your general rules higher in the stylesheet, and your more specific rules towards the bottom. Some people think the Cascade is a very frustrating part of web design, but it can be a useful design tool if applied carefully!

The source code provided with this tutorial includes a wide range of rules that designate how page elements should look. These properties include spacing, coloring, reactions to hovering, animations, sizing, and more. We'll dive into the source code and examine what some of the common properties are. 

There are too many CSS properties to memorize - [336](http://meiert.com/en/indices/css-properties/) as of August 10, 2015. Don't worry about memorizing them all- you'll learn the important ones from reading code and building basic websites! 

> Explore `styles.css` as time permits.

_I heard we can sneak styles directly onto an html page. Why are we doing this?_
> Short answer for beginners: It's better for modularity and makes your code more reusable. It also makes life easier for search engines.
For advanced users: Styles at the head of the document: do it to improve pageload time. Only use the styles that affect the image above the fold, then put the stylesheet at the end of the page together with your script imports. This will minimize the time the user gets a blank screen, and defers loading the rest of the styles until the first screen area has been properly formatted.

_Why don't we edit the styles directly on the HTML element? `style` attribute is dying to be used!_
> Inline styles are BAD PRACTICE, but they technically work. They are used in niche applications such as html in emails, since you can't link to stylesheets for security reasons

### Sparks Fly: A dose of Javascript

Javascript is the scripting language of the internet. Every web browser has a javascript console that can play with.

> Cue Chrome Developer Console.

You can import an external library but it may have more code than you need, and you need to trust that the provider isn't doing anything malicious or won't be compromised. It's usually safe, but it's good to avoid unnecessary risk!

_I don't want to make a separate file! Can I put my scripts on the html page?_
> Inline scripts are possible but discouraged. If for some reason you can't link to an external js file, you can put them on the html page inside `script` tags.

#### Examining the Code for a Sticky Header

Let's look at the code living in `main.js`. We want to add a neat effect for when people scroll down the page.

Design Logic
+ Watch something about the page or window
+ Select something when changes are detected to that watched something
+ Make something cool happen!

```js
window.onscroll = function() {
  var el = document.getElementsByClassName('header')[0];
  var className = 'small';
  if (el.classList) {
    if (window.scrollY > 10)
      el.classList.add(className);
    else
      el.classList.remove(className);
  }
};
```
> Show how to link to scripts

```html
    <html>
        <head>
            <!-- Header code -->
        </head>
        <body>
            ...
            <!-- all your great html code -->
            <script type="text/javascript" src="main.js"></script>
        </body>
    </html>
```
Challenge: What would you do to change the header COLOR on scroll instead of header HEIGHT?

Wow! You've finished your first website! Let's see what kinds of things there are left to learn!

###Next: [Ignition](ignition.md)