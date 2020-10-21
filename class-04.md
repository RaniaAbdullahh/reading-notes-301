## Regex 
- ## what is Regex 

Regular expressions (regex or regexp) are extremely useful in extracting information from any text by searching for one or more matches of a specific search pattern (i.e. a specific sequence of ASCII or unicode characters).
Fields of application range from validation to parsing/replacing strings, passing through translating data to other formats and web scraping.
One of the most interesting features is that once you’ve learned the syntax, you can actually use this tool in (almost) all programming languages ​​(JavaScript, Java, VB, C #, C / C++, Python, Perl, Ruby, Delphi, R, Tcl, and many others) with the slightest distinctions about the support of the most advanced features and syntax versions supported by the engines).
> Ex:

- Anchors — ^ and $
``^The        matches any string that starts with The ->`` 
  ``end$        matches a string that ends with end``
  
- Quantifiers — * + ? and {} 
``abc+        matches a string that has ab followed by one or more c``
``abc?        matches a string that has ab followed by zero or one c``

- Character classes — \d \w \s and .
``\w         matches a word character (alphanumeric character plus underscore) ->``
- Bracket expressions — []  ``[abc]            matches a string that has either an a or a b or a c -> is the same as a|b|c ->``
- Look-ahead and Look-behind — (?=) and (?<=)
``d(?=r)       matches a d only if is followed by r, but r will not be part of the overall regex match ->``

## Common Responsive Layouts with CSS Grid
The smaller images (in a grid!) are in the perfect layout to get you started with CSS grid. Grid gives us control over how wide or narrow each of the ‘grid cells’ get. This allows us to maintain a sensible aspect ratio to their height. In this example I’ve used:
``grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));``
- The Full Page Image Gallery
to  create a grid with 6 columns which are each one fraction unit wide. They each share 1/6 of the width of the container use :
``grid-template-columns: 1fr 1fr 1fr 1fr 1fr 1fr;``
- Card Layout
This is a column layout that fills each column with cards as the screen width increases. This is a great example of where, in my opinion, grid is not necessarily required. Here we have a column layout that is filling up with cards. We don’t necessarily know the size of each card, nor do we need the other card heights to change if a card is particularly tall. CSS colums are designed to do this.
``column-count: 2;``
``column-gap: 20px;``
## Grid
- display
``.container {
  display: grid | inline-grid;
}``
