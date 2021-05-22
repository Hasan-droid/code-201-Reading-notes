# 1. Transforms

![img](https://www.edureka.co/blog/wp-content/uploads/2019/09/Transform-CSS.jpg)

With CSS3 came new ways to position and alter elements. Now general layout techniques can be revisited with alternative ways to size, position, and change elements. All of these new techniques are made possible by the transform property.

The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.

Within this lesson we’ll take a look at both two-dimensional and three-dimensional transforms. Generally speaking, browser support for the transform property isn’t great, but it is getting better every day. For the best support vendor prefixes are encouraged, however you may need to download the nightly version of Chrome to see all of these transforms in action.

Transform Syntax The actual syntax for the transform property is quite simple, including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses.

## 2D Transforms

Elements may be distorted, or transformed, on both a two-dimensional plane or a three-dimensional plane. Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes. Three-dimensional transforms work on both the x and y axes, as well as the z axis. These three-dimensional transforms help define not only the length and width of an element, but also the depth. We’ll start by discussing how to transform elements on a two-dimensional plane, and then work our way into three-dimensional transforms.

## 2D Rotate

The transform property accepts a handful of different values. The rotate value provides the ability to rotate an element from 0 to 360 degrees. Using a positive value will rotate an element clockwise, and using a negative value will rotate the element counterclockwise. The default point of rotation is the center of the element, 50% 50%, both horizontally and vertically. Later we will discuss how you can change this default point of rotation.

## 2D Scale

Using the scale value within the transform property allows you to change the appeared size of an element. The default scale value is 1, therefore any value between .99 and .01 makes an element appear smaller while any value greater than or equal to 1.01 makes an element appear larger.

Transitions & Animations One evolution with CSS3 was the ability to write behaviors for transitions and animations. Front end developers have been asking for the ability to design these interactions within HTML and CSS, without the use of JavaScript or Flash, for years. Now their wish has come true.

## 2. Transitions

![img](https://www.problogdesign.com/wp-content/uploads/2013/01/css3-transitions2.jpg)

 To alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted.<br>
 There are four transition related properties
 1. transition-property
 2. transition-duration
 3. transition-timing-function
 4. transition-delay<br>

 - ### transition-property<br>
 The transition-property property determines exactly what properties will be altered in conjunction with the other transitional properties<br>
 If multiple properties need to be transitioned they may be comma separated within the transition-property value<br>


- ### transition-duration
The duration in which a transition takes place is set using the transition-duration property.<br>
- ### transition-timing-function
The transition-timing-function property is used to set the speed in which a transition will move. <br>
- ### transition-delay
The delay sets a time value, seconds or milliseconds, that determines how long a transition should be stalled before executing.<br>


<br>
<br>
<hr>

