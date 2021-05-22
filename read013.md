## LOCAL STORAGE FOR WEB APPLICATIONS
ersistent local storage is one of the areas where native client applications have held an advantage over web application
####  can be used for persistent local storage of small amounts of data. But they have three potentially dealbreaking downsides:
* Cookies are included with every HTTP request,
* Cookies are included with every HTTP request
* Cookies are limited to about 4 KB of data

### What we really want is?
a lot of storage spaceon the client that persists beyond a page refresh and isn’t transmitted to the server

### A BRIEF HISTORY OF LOCAL STORAGE HACKS BEFORE HTML5
microsoft invented a great many things and included them in their browser-to-end-all-browser-wars, Internet Explorer.examble of thses things 
* DHTML Behaviors,
* userData:userData allows web pages to store up to 64 KB of data per domain
### A BRIEF HISTORY OF LOCAL STORAGE HACKS BEFORE HTML5
In 2002, Adobe introduced a feature in Flash 6 that gained the unfortunate and misleading name of “Flash cookies.”
In 2007, Google launched Gears, an open source browser plugin aimed at providing additional capabilities in browsers.
By 2009, dojox.storage could auto-detect (and provide a unified interface on top of) Adobe Flash, Gears
*they all expose radically different interfaces, have different storage limitations, and present different user experiences. So this is the problem that HTML5 set out to solve
HTML5 STORAGE*
### INTRODUCING HTML5 STORAGE
it’s a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies

### USING HTML5 STORAGE
HTML5 Storage is based on named key/value pairs. You store data based on a named key, 
There are also methods for removing the value for a given named key, and clearing the entire storage area (that is, deleting all the keys and values at once).
Finally, there is a property to get the total number of values in the storage area, and to iterate through all of the keys by index (to get the name of each key).

### TRACKING CHANGES TO THE HTML5 STORAGE AREA
If you want to keep track programmatically of when the storage area changes, you can trap the storage event. 
 with HTML5 Storage, we can save the progress locally, within the browser itself
the present condition of HTML5 Storage is surprisingly rosy. A new API has been standardized and implemented across all major browsers, platforms, and devices. 

### STORAGEEVENT OBJECT
PROPERTY TYPE DESCRIPTION key string the named key that was added, removed, or modified oldValue any the previous value (now overwritten), or null if a new item was added newValue any the new value, or null if an item was removed url* string the page which called a method that triggered this change


### BEYOND NAMED KEY-VALUE PAIRS: COMPETING VISIONS
While the past is littered with hacks and workarounds, the present condition of HTML5 Storage is surprisingly rosy. A new API has been standardized and implemented across all major browsers, platforms, and devices. As a web developer, that’s just not something you see every day, is it? But there is more to life than “5 megabytes of named key/value pairs,” and the future of persistent local storage is… how shall I put it… well, there are competing visions.