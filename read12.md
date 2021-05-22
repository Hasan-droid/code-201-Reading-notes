![img](https://miro.medium.com/max/902/1*CPSTzfUTCCpUbllyiPvl_A.jpeg)

## CHART JS

1. Getting Started
First, we need to have a canvas in our page. next include Chart.js then add a script .
2. Installation
Chart.js can be installed via npm or bower. It is recommended to get Chart.js this way.
3. Integration
Chart.js can be integrated with plain JavaScript or with different module loaders.
4. Usage
Chart.js can be integrated with plain JavaScript or with different module loaders. The examples below show how to load Chart.js in different systems.

### Charts

Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier
to look at and convey data quickly, but they’re not always easy to create.

### Setting up

The first thing we need to do is download Chart.js. Copy the Chart.min.js out of the unzipped folder and into the directory you’ll be working in. Then create a new html page and
import the script.

### Drawing a line chart

To draw a line chart, the first thing we need to do is create a canvas element in our HTML in which Chart.js can draw our chart. So add this to the body of our HTML page

### Drawing a pie chart

 1. First, we need the canvas element
 2. Next, we need to get the context and to instantiate the chart:
 3. Next we need to create the data. This data is a little different to the line chart because the pie chart is simpler, we just need to supply a value and a color for each

### Basic usage of canvas

At first sight a < canvas> looks like the < img> element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the < canvas> element has
only two attributes, width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will
initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily by CSS, but during rendering the image is scaled to fit its layout size: if the CSS sizing
doesn't respect the ratio of the initial canvas, it will appear distorted.

The id attribute isn't specific to the < canvas> element but is one of the global HTML attributes which can be applied to any HTML element (like class for instance). It is
always a good idea to supply an id because this makes it much easier to identify it in a script

### Fallback content

The < canvas > element differs from an  < img > tag in that, like for < video >, < audio >, or < picture > elements, it is easy to define some fallback content, to be displayed
 in older browsers not supporting it, like versions of Internet Explorer earlier than version 9 or textual browsers.

#### The rendering context:The < canvas > element creates a fixed-size drawing surface that exposes one or more rendering contexts

#### Checking for support:Scripts can also check for support programmatically by testing for the presence of the getContext() method

### Drawing shapes with canvas

#### The grid

Before we can start drawing, we need to talk about the canvas grid or coordinate space. Our HTML skeleton from the previous page had a canvas element 150 pixels wide and 150
pixels high. The origin of this grid is positioned in the top left corner at coordinate (0,0). All elements are placed relative to this origin. So the position of the top left
corner of a square becomes x pixels from the left and y pixels from the top, at coordinate (x,y).

### Drawing rectangles

here are three functions that draw rectangles on the canvas:

* fillRect(x, y, width, height)
Draws a filled rectangle.
* strokeRect(x, y, width, height)
Draws a rectangular outline.
* clearRect(x, y, width, height)
Clears the specified rectangular area, making it fully transparent.

### Drawing paths

Now let's look at paths. A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color. A
path, or even a subpath, can be closed. To make shapes using paths, we take some extra steps:

* First, you create the path.
* Then you use drawing commands to draw into the path.
* Once the path has been created, you can stroke or fill the path to render it.

### Moving the pen

One very useful function, which doesn't actually draw anything but becomes part of the path list described above, is the moveTo() function. You can probably best think of this
as lifting a pen or pencil from one spot on a piece of paper and placing it on the next.

#### moveTo(x, y) :Moves the pen to the coordinates specified by x and y

### Lines

For drawing straight lines, use the lineTo() method. lineTo(x, y)

### Arcs

To draw arcs or circles, we use the arc() or arcTo() methods:arc(x, y, radius, startAngle, endAngle, anticlockwise)

### Bezier and quadratic curves

The next type of paths available are Bézier curves, available in both cubic and quadratic varieties. These are generally used to draw complex organic shapes.

### Path2D objects

 there can be a series of paths and drawing commands to draw objects onto your canvas. To simplify the code and to improve performance, the Path2D object, available in recent
 versions of browsers.

### Using SVG paths

 is using SVG path data to initialize paths on your canvas. This might allow you to pass around path data and re-use them in both, SVG and canvas.

## Applying styles and colors

### Colors

* fillStyle = color   to sets the style used when filling shapes.
* strokeStyle = color  to sets the style for shapes' outlines.

### Transparency

 we can also draw semi-transparent (or translucent) shapes. This is done by either setting the globalAlpha property or by assigning a semi-transparent color to the stroke and/or
 fill style. ```globalAlpha = transparencyValue```

### Using rgba()

Using rgba() gives you a little more control and flexibility because we can set the fill and stroke style individually.

### Line styles

#### There are several properties which allow us to style lines

* lineWidth = value
Sets the width of lines drawn in the future.
* lineCap = type
Sets the appearance of the ends of lines.
* lineJoin = type
Sets the appearance of the "corners" where lines meet.
* miterLimit = value
Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.

### getLineDash()

Returns the current line dash pattern array containing an even number of non-negative numbers.

### setLineDash(segments)

Sets the current line dash pattern.
lineDashOffset = value
Specifies where to start a dash array on a line.

### A demo of the miterLimit property

The miterLimit property determines how far the outside connection point can be placed from the inside connection point

### Using line dashes

The setLineDash method and the lineDashOffset property specify the dash pattern for line.

### Gradients

1. createLinearGradient(x1, y1, x2, y2)
2. Creates a linear gradient object with a starting point of (x1, y1) and an end point of (x2, y2).
3. createRadialGradient(x1, y1, r1, x2, y2, r2)
4. Creates a radial gradient. The parameters represent two circles, one with its center at (x1, y1)  and a radius of r1, and the other with its center at (x2, y2) with a radius
of r2.
6. createConicGradient(angle, x, y)
7. Creates a conic gradient object with a starting angle of angle in radians, at the position (x, y).

### Patterns

In one of the examples on the previous page, we used a series of loops to create a pattern of images. There is, however, a much simpler method: the createPattern() method.

* repeat
Tiles the image in both vertical and horizontal directions.
* repeat-x
Tiles the image horizontally but not vertically.
* repeat-y
Tiles the image vertically but not horizontally.
* no-repeat
Doesn't tile the image. It's used only once.

### Shadows

* shadowOffsetX = float
* shadowOffsetY = float
* shadowBlur = float
* shadowColor = color

## Drawing text

#### fillText(text, x, y [, maxWidth])

Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.

#### strokeText(text, x, y [, maxWidth])

Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

### Styling text

* font = value
The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.
* textAlign = value
Text alignment setting. Possible values: start, end, left, right or center. The default value is start.
* textBaseline = value
Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.
* direction = value
Directionality. Possible values: ltr, rtl, inherit. The default value is inherit.

### Advanced text measurements

In the case you need to obtain more details about the text, the following method allows you to measure it. measureText().