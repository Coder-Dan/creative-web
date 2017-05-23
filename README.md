# About this Web site

## Preface

I had change of heart. I like to keep my project to myself but then no one will ever see the work I can do. So this is will be my first project that I'll be putting out in the open. So you can fork it, recommend edits or use it as a basis for your own project - I'll be learning from developing and hopefully this action leads to an improved independant and continuous development that is outside of work and univeristity.

## Project Description

### How have I build it?

* With sheer tenacity :). No but really, I did have a lot of drive when I start. I just keep writing and writing, looking up stuff on the internet and just reading and applying what I've seen. I do actually have some design documents on paper for the layout of the website.

* Building in **In Stages**:
    * Over the development process, I've been reading new resources and applying my code here to test new development and understand web code examples.
    * Periodically, I make new updates to this website to learn some more HTML and CSS tricks to apply. But my goal was to understand how program a good website design is programmed, and understand how to manipulated it to a simple designs of my own.
    * At the moment I'm yet to include some JavaScript and I'm leaving web services to last - just to focus on design and structuring HTML pages.

### What is this website?

* This website is designed to be as personal website for professional profile, it will be leaning more for programmers and developers, **as of May 2017, and can be subject to change**.

## Documentation

Here I'll write stuff about topic I've looked to understand and implement. Most of the stuff I write here, means that I've also implemented in this code.

### CSS Box Model Notes
![Box Model](https://i.stack.imgur.com/Rs3Rb.png)
#### 'Background colour not including margin space'
* Using 'Margin space' will not be included as part of the element area and therefore will **not** be coloured. Though, upon analysis, it takes up the space you set with margin but that space isn't seen as part of the element contents (defined as the inside of the border). Hence, the container will also act the same way and will not colour that space.

* Solution is to use **padding** as it adds space inside element box; the container will also see this and colour the area underneath, or in better terms, as defined by the padding.

```HTML 
<p style= "margin: 0; padding-bottom: 10px;">Powered by Caffine!</p>
```

* Think about this further, how do the side margin get colored in but bottom ones, when we are not careful, do not? It lies in the fact colouring is dependant on the area defined by padding and content; if an area is defined by that then it is colored. So when you create an inner element and define some side margins, **inner element's margins are coloured by the parent element**. Thinking about this further, if you extend an container element's bottom padding to include margin of it's last inner element - you effectively colour the margin for that area.

```HTML
        <!--FOOTER code-->
        <footer>
            <div class="footer-container">
                <h2>Daniel A. Minero</h2>
                <p>Webcode provided on <a href="http://github.com/Coder-Dan/creative-website">GitHub</a></p>
                <p style="margin: 10px; padding-bottom: 0px">Powered by Caffine and Biscuits!</p>
            </div>
        </footer>
```

```css
footer {
    background: lightslategrey;
    padding-bottom: 10px;
    /* Adding padding to compensate for extra margin at the bottom, 
     * bootstrap adds 10px bottom margin to <p> tags; so i did the same with inline style*/
}

.footer-container {
    padding-right: 15px;
    padding-left: 15px;
    margin-right: auto;
    margin-left: auto;
}
```

## References

Keeping a list of wonderful reference over the journey you can head on down to, if want something to get started on.

### Websites

* Referenced Template design for Developer CVs by 'xriley' on [GitHub](https://github.com/xriley/Orbit-Theme)
* [Understanding CSS **Position** Attribute](https://www.w3schools.com/cssref/playit.asp?filename=playcss_position)
* [This is Responsive Web Design - Code Pattern Samples](http://bradfrost.github.io/this-is-responsive/)
* [How to Build Websites](http://www.how-to-build-websites.com/) - by the same guy who wrote 'Web Design start here'
* [Start Here](http://www.webdesignstarthere.com)
* [How to learn a new programming language](http://www.killersites.com/blog/2017/how-to-learn-a-new-programming-language/)

### Stack Overflow
* [Understanding bootstrap 3 column layout changes, with respect to screeen size](http://stackoverflow.com/questions/20767594/what-does-this-mean-in-bootstrap-3-docs)
* [Centering elements in CSS](http://stackoverflow.com/questions/79461/vertical-alignment-of-elements-in-a-div) - need some sample implementation code


### Books

* Mischook, S. (2015). _Web design start here: all you need to create your own fantastic websites_ (1st ed.). Cambridge: Ilex
* Moore, A. (2016). _Create your own website the easy way_. London: ILEX, a division of Octopus Publishing Group Ltd.

### Website designs

* [Bootstrap 'dashboard' theme + docs](https://bootstrap-themes.github.io/dashboard/docs/)

## Frequentally Useful Resources

* [List of all HTML Tags](https://www.w3schools.com/tags/default.asp) identifies HTML5 specific tags and depreciated tags
* [CSS Tricks](https://css-tricks.com/almanac/properties/t/transition/)
* [MDN Web Development Tutorial](https://developer.mozilla.org/en-US/docs/Learn) - Mozilla Network is well maintained and documented site for Web Developers to learn and understand web dev (HTML, CSS, JS, etc.); regarded as one of the best places to start for reading more into specific topics. I've linked the MDN tutorial for web development, it also for complete beginners.
* [Wireframing](http://uxmovement.com/content/why-you-should-never-center-align-paragraph-text/)
* [Bootstrap 'Kitchen Sink' - All HTML elements in one page](https://bootstrap-themes.github.io/dashboard/bootstrap/index.html)
* 
