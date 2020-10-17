## Responsive Web Design
Responsive web design is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop. Responsive web design is focused around providing an intuitive and gratifying experience for everyone. Desktop computer and cell phone users alike all benefit from responsive websites.

1. Flexible Layouts

Responsive web design is broken down into three main components, including flexible layouts, media queries, and flexible media. The first part, flexible layouts, is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width. Flexible grids are built using relative length units, most commonly percentages or em units.
These relative lengths are then used to declare common grid property values such as ``width``,`` margin``, or ``padding.``

2. Media Queries

There are a couple different ways to use media queries, using the @media rule inside of an existing style sheet, importing a new style sheet using the @import rule, or by linking to a separate style sheet from within the HTML document.
Generally speaking it is recommend to use the @media rule inside of an existing style sheet to avoid any additional HTTP requests.

>Logical Operators in Media Queries
Using the and logical operator within a media query allows an extra condition to be added, making sure that a browser or devices does both a, b, c, and so forth.
Multiple individual media queries can be comma separated, acting as an unspoken or operator.
The example below selects all media types between 800 and 1024 pixels wide.

3. Mobile First

The mobile first approach also advocates designing with the constraints of a mobile user in mind. Before too long, the majority of Internet consumption will be done on a mobile device. 
Plan for them accordingly and develop intrinsic mobile experiences.

`` @media screen and (min-width: 400px)  {...}
@media screen and (min-width: 600px)  {...}
``

4. Flexible Media
The final, equally important aspect to responsive web design involves flexible media. As viewports begin to change size media doesn’t always follow suit. Images, videos, and other media types need to be scalable, changing their size as the size of the viewport changes.

One quick way to make media scalable is by using the max-width property with a value of 100%. Doing so ensures that as the viewport gets smaller any media will scale down according to its containers width.
``
img, video, canvas {
  max-width: 100%;
}
``

## All About Floats
Float is a CSS positioning property. To understand its purpose and origin, we can look to print design.
In a print layout, images may be set into the page such that text wraps around them as needed.
>Setting the float on an element with CSS happens like this:
``
#sidebar {
  float: right;			
}
``
# What are floats used for?
- floats can be used to create entire web layouts.
- Floats are also helpful for layout in smaller instances. 

# Clearing the Float
Float’s sister property is clear. An element that has the clear property set on it will not move up adjacent to the float like the float desires
``
#footer {
  clear: both;			
}
``
# The Great Collapse
One of the more bewildering things about working with floats is how they can affect the element that contains them (their “parent” element). If this parent element contained nothing but floated elements, the height of it would literally collapse to nothing.
This isn’t always obvious if the parent doesn’t contain any visually noticeable background, but it is important to be aware of.

# Techniques for Clearing Floats
- The Empty Div Method is, quite literally, an empty div.`` <div style="clear: both;"></div>. ``
- The Overflow Method relies on setting the overflow CSS property on a parent element. If this property is set to auto or hidden on the parent element, the parent will expand to contain the floats, effectively clearing it for succeeding elements. This method can be beautifully semantic as it may not require additional elements. However if you find yourself adding a new div just to apply this, it is equally as non-semantic as the empty div method and less adaptable.
Also bear in mind that the overflow property isn’t specifically for clearing floats.
- The Easy Clearing Method uses a clever CSS pseudo selector (:after) to clear floats.
``
.clearfix:after { 
   content: "."; 
   visibility: hidden; 
   display: block; 
   height: 0; 
   clear: both;
}
``
