# links
its the way web pages uses to quicly surf the webpage itself or to redirect from a wep page to another
>Links are the defining feature of the web
because they allow you to move from
one web page to another — enabling the
very idea of browsing or surfing.
1. **linking to other sites**:
* \<a href="http://www.empireonline.com">empireonline\</a>
2. **Linking to Other Pageson the Same Site**
* \<a href="index.html">Home\</a>
3. **Directory Structure**
   1. **Child Folder** :\<a href="music/listings.html">Listings\</a>
   2. **Parent Folder** :Use ../ to indicate the folder above the current one,
then follow it with the file name.

      \<a href="../../index.html">Home\</a>
4. **Email Links**: \<a href="mailto:jon@example.org">Email Jon\</a>
5. **Opening Links ina New Window**:\<a href="http://www.imdb.com" target="_blank">
Internet Movie Database\</a>
> Generally you should avoid
opening links in a new window,
but if you do, it is considered
good practice to inform users
6. **Linking to a Specific Part of the Same Page**:

\<a href="#arc_shot">Arc Shot\</a>
\<h2 id="arc_shot">Arc Shot\</h2>
7. **Linking to a Specific Part of Another Page** :
\<a href="http:/www.htmlandcssbookcom/#bottom">
> Therefore, the href attribute will contain the address for the page (either an absolute URL or a relative URL), ollowed by the # symbol, followed by the value of the id attribute that is used on

# positioning elements
* **Block-level elements**:\<h1> \<p> \<ul> \<li>
* **Inline elements**:\<img> \<b> \<i>
1. **Containing Elements**
> If one block-level element sits inside another
block-level element then the outer box is
known as the containing or parent element.
> The \<div> element that contains this group of
elements is then referred to as the containing element.

2. **Controlling the Position of Elements**:
> * Normal flow
Every block-level elementappears on a new line, causing
each item to appear lower down the page than the previous one. 
> * Relative Positioning This moves an element from the
position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed. *This does not affect the position of surrounding elements;*
> * Absolute positioning This positions the element in relation to its containing element. It is taken out of
normal flow, meaning that it does not affect the position
of any surrounding elements 

> * Fixed Positioning This is a form of absolute positioning that positions the element **in relation to the browser window,** as opposed to the containing element.
>* Floating Elements
Floating an element allows
you to take that element out
of normal flow and position
it to the far left or right of a
containing box
>* **When you move
any element from
normal flow, boxes
can overlap. The
z-index property
allows you to control
which box appears
on top.**

