## Making Modern Websites: Basic Site

We've come a long way since the websites of the 90s! What changed?
> While waiting, checkout these blasts from the [past](http://retrosite.ninja/)!

![Facebook before](http://cnet1.cbsistatic.com/hub/i/r/2014/02/03/f1e9d629-a5c4-11e3-a24e-d4ae52e62bcc/resize/1170x878/5c34b29efda0801143249cc83b048e75/2005_17.jpg)

In other cases...
+ [Greenlight Capital](https://www.greenlightcapital.com/) (Worth $10 Billion)
+ [Berkshire Hathaway](http://www.berkshirehathaway.com/) (Website of the world's wealthiest man)

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

We will be using a combination of <div>

####Part 2: Using Components

### Sparkly Sparks: CSS for Styles

CSS is younger than HTML!

![Anatomy of a rule](http://ironion.com/wp-content/uploads/2015/06/cssanatomy1.png)

#### Part 1: Learn the ABCs: CSS Declarations
+ Breaking Down the Stylesheet + Cascading Effect
+ Selectors: ELements, .Classes, and #IDs
+ Selectors: Chaining Selectors
+ CSS Styles: Google them and learn by doing

_I heard we can sneak styles directly onto an html page. Why are we doing this?_
> Short answer for beginners: It's better for modularity and makes your code more reusable. It also makes life easier for search engines.
For advanced users: Styles at the head of the document: do it to improve pageload time. Only use the styles that affect the image above the fold, then put the stylesheet at the end of the page together with your script imports. This will minimize the time the user gets a blank screen, and defers loading the rest of the styles until the first screen area has been properly formatted.

_Why don't we edit the styles directly on the HTML element? `style` attribute is dying to be used!_
> Inline styles are BAD PRACTICE, but they technically work. They are used in niche applications such as html in emails, since you can't link to stylesheets for security reasons

### Sparks Fly: A dose of Javascript

Javascript is the scripting language of the internet. Every web browser has a javascript console that can play with.

> Cue Chrome Developer Console.

You can import an external library but it may have more code than you need, and you need to trust that the provider isn't doing anything malicious without telling you.

_I don't want to make a separate file! Can I put my scripts on the html page?_
> Inline scripts are possible but discouraged. If for some reason you can't link to an external js file, you can put them on the html page inside `script` tags.

#### Examining the Code for a Sticky Header

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

Challenge: What would you do to change the header COLOR on scroll instead of header HEIGHT?

Wow! You've finished your first website! Let's see what kinds of things you can learn next.

###Next: [Ignition](ignition.md)