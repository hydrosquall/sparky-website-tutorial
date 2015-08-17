## Making Modern Websites: Basic Site

We've come a long way since the websites of the 90s! What changed?
> While waiting, checkout these blasts from the [past](http://retrosite.ninja/)!

![Facebook before](http://cnet1.cbsistatic.com/hub/i/r/2014/02/03/f1e9d629-a5c4-11e3-a24e-d4ae52e62bcc/resize/1170x878/5c34b29efda0801143249cc83b048e75/2005_17.jpg)

In other cases...
[Greenlight Capital](https://www.greenlightcapital.com/) (Worth $10 Billion)
[Berkshire Hathaway](http://www.berkshirehathaway.com/) (Website of the world's wealthiest man)

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

We will be using `<div>` tags, 

####Part 2: Using Components

### Sparkly Sparks: CSS for Styles

Didn't exist at first. 

Breaking Down the Stylesheet + Cascading Effect

Selectors

> advanced: Styles at the head of the document: do it for pageload time for above the fold

Inline styles are BAD PRACTICE, but they technically work. They are used for niche applications such as html in emails, since you can't link to stylesheets in emails.

### Sparks Fly: Tricks with Javascript

Many ways to do the same thing. Usually hook things with IDs, faster than classes.

You can import an external library but it may have more code than you need, and you need to trust that the provider isn't doing anything malicious without telling you.


Inline scripts are possible but discouraged. If for some reason you can't link to an external js file, you can put them on the html page inside `script` tags.



### Pyromania: Javascript Logic with Sticky Header