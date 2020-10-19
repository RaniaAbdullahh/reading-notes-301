## what is jQuery
jQuery is  JavaScript library that is based on its motto "write less, do more". jQuery is a fast, small, and feature-rich JavaScript library.
It makes things like HTML document traversal and manipulation, event handling, and animation much simpler.

# WHY USE JQUERY
first you shoud script Jqury library by ``<script src="j s/ jquery-1 .11. 0 .js "></script>``

1-SIMPLE SELECTORS

Selecting the elements through a typical JavaScript approach could be very painful, but the jQuery works like a magic here. The ability of making the DOM elements selection simple and easy is one of the most powerful feature of the jQuery.

2-COMMON TASKS IN LESS CODE

jQuery considerably simplifies the common JavaScript tasks. Now you can easily create feature rich and interactive web pages with fewer lines of codes.

3-CROSS-BROWSER COMPATIBILITY

jQuery is created with modern browsers in mind and it is compatible with all major modern browsers such as Chrome, Firefox, Safari, Internet Explorer, etc. A jQuery statement typically starts with the dollar sign ($) and ends with a semicolon (;). In jQuery, the dollar sign ($) is just an alias for jQuery.

BASIC EFFECTS
In this example, it appears as if list items are faded into view when the page loads. Each item is faded out when it is clicked on. ``$(function() { $('h2').hide().slideDown(); var $li = $('li'); $li.hide().each{function(index) { 2 $(this).delay(700 * index) .fadeln(?OO); } ) ; 3 $li.on('click', function() $(this) .fade0ut(700); } ) ; });``

## Six Reasons for Pair Programming

1. Greater efficiency
It is a common misconception that pair programming takes a lot longer and is less efficient. In reality, when two people focus on the same code base, it is easier to catch mistakes in the making.

2. Engaged collaboration
When two programmers focus on the same code, the experience is more engaging and both programmers are more focused than if they were working alone.

3. Learning from fellow students
Everyone has a different approach to problem solving; working with a teammate can expose developers to techniques they otherwise would not have thought of.

4. Social skills
Pair programming is great for improving social skills. When working with someone who has a different coding style, communication is key. This can become more difficult when two programmers have different personalities.

5. Job interview readiness
A common step in many interview processes involves pair programming between a current employee and an applicant, either in person or through a shared screen. They will carry out exercises together, such as code challenges, building a project or feature, or debugging an existing code base.

6. Work environment readiness
Many companies that utilize pair programing expect to train fresh hires from CS-degree programs on how they operate to actually deliver a product. Code Fellows graduates who are already familiar with how pairing works can hit the ground running at a new job, with one less hurdle to overcome.


