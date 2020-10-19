## Javascript Templating

Javascript templating is a fast and efficient technique to render client-side view templates with Javascript by using a JSON data source. The template is HTML markup, with added templating tags that will either insert variables or run programming logic.
>Mustache
 is a logic-less template syntax. It can be used for HTML, config files, source code — anything. It works by expanding tags in a template using values provided in a hash or object.
 - mustache.js
 is an implementation of the mustache template system in JavaScript. It is often considered the base for JavaScript templating. And, since mustache supports various languages, we don’t need a separate templating system on the server side.
 ``Mustache.render(“Hello, {{name}}”, { name: “Sherlynn” });
// returns: Hello, Sherlynn``
# Mustache-Express
Mustache Express lets you use Mustache and Express together easily.
- To install:
``$ npm install mustache --save``
-  Example:
``res.render('hello', {"name": "Sherlynn"})`` => Whereby the first parameter ‘hello’ refers to the hello.html file (no need to include the extension (e.g. hello.html) as it has been previously set as html.
The second parameter would be the JSON data itself. 

## A Complete Guide to Flexbox
### 1. Properties for the Parent (flex container)
- display
This defines a flex container; inline or block depending on the given value. It enables a flex context for all its direct children.
``.container { display: flex; /* or inline-flex */}``
- flex-direction
``.container { flex-direction: row | row-reverse | column | column-reverse;}``
>row (default): left to right in ltr; right to left in rtl

>row-reverse: right to left in ltr; left to right in rtl

>column: same as row but top to bottom

>column-reverse: same as row-reverse but bottom to top

- flex-wrap
``.container {flex-wrap: nowrap | wrap | wrap-reverse;}``
>nowrap (default): all flex items will be on one line

>wrap: flex items will wrap onto multiple lines, from top to bottom.

>wrap-reverse: flex items will wrap onto multiple lines from bottom to top.
- flex-flow
``.container {flex-flow: column wrap;}``
-justify-content

``.container {justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly | start | end | left | right ... + safe | unsafe;}``
- align-items

``.container {align-items: stretch | flex-start | flex-end | center | baseline | first baseline | last baseline | start | end | self-start | self-end + ... safe | unsafe;}``
- align-content
``.container { align-content: flex-start | flex-end | center | space-between | space-around | space-evenly | stretch | start | end | baseline | first baseline | last baseline + ... safe | unsafe;}``
### 2. Properties for the Children (flex items)
- order
>By default, flex items are laid out in the source order.

``.item { order: 5; /* default is 0 */}``

- flex-grow
>This defines the ability for a flex item to grow if necessary.

``.item {flex-grow: 4; /* default 0 */}``

- flex-shrink
>This defines the ability for a flex item to shrink if necessary.

``.item { flex-shrink: 3; /* default 1 */}``
- flex
> This is the shorthand for flex-grow, flex-shrink and flex-basis combined. 

``.item {flex: none | [ <'flex-grow'> <'flex-shrink'>? || <'flex-basis'> ]}``
- align-self

``item { align-self: auto | flex-start | flex-end | center | baseline | stretch;}``

