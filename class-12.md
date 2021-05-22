## API

#### The **canvas** element
`<canvas id="tutorial" width="150" height="150"></canvas>`
####  the *canvas* element has only two attributes, width and height
#### The *canvas* element differs from an *img* tag in that, like for *video*, *audio*, or *picture* elements, it is easy to define some fallback content, to be displayed in older browsers not supporting it,
#### The *canvas* element creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown. 

![Canvas](https://www.researchgate.net/profile/Curran-Kelleher/publication/262398551/figure/fig5/AS:666687049306144@1535961987543/Example-code-for-HTML5-Canvas.png)

#### only supports two primitive shapes :
1. rectangles 
2. paths

#### A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color.

#### there can be a series of paths and drawing commands to draw objects onto your canvas. To simplify the code and to improve performance, the Path2D object, available in recent versions of browsers,

##### Example :

![Path2D](https://mdn.mozillademos.org/files/9851/path2d.png)


#### Example using color in canvas :
###### function draw() {var ctx = document.getElementById('canvas').getContext('2d');for (var i = 0; i < 6; i++) { for (var j = 0; j < 6; j++) {  ctx.fillStyle = 'rgb(' + Math.floor(255 - 42.5 * i) + ', ' + Math.floor(255 - 42.5 * j) + ', 0)';ctx.fillRect(j * 25, i * 25, 25, 25);}}}


#### In addition to drawing opaque shapes to the canvas, we can also draw semi-transparent (or translucent) shapes


#### The canvas rendering context provides two methods to render text:

###### fillText(text, x, y [, maxWidth])

`ctx.font = '48px serif'; ctx.textBaseline = 'hanging'; ctx.strokeText('Hello world', 0, 100);`