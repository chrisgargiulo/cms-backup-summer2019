---
ID: 1597
post_title: 'JS Basics: Functions and Syntax'
author: Java Joe
post_excerpt: ""
layout: post
permalink: >
  https://www.creativemedia.space/js-basics-functions-syntax-and-common-uses/
published: true
post_date: 2018-02-15 15:42:09
---
[et_pb_section bb_built="1" fullwidth="off" specialty="off" next_background_color="#000000"][et_pb_row][et_pb_column type="4_4"][et_pb_image _builder_version="3.0.101" src="https://www.creativemedia.space/wp-content/uploads/2018/02/js-4x2.gif" show_in_lightbox="off" url_new_window="off" use_overlay="off" always_center_on_mobile="on" force_fullwidth="off" show_bottom_space="on" /][/et_pb_column][/et_pb_row][et_pb_row][et_pb_column type="4_4"][et_pb_text admin_label="Running Head" _builder_version="3.0.92" background_layout="light" module_class="articlerunninghead text-single-column-narrow"]

Lesson

[/et_pb_text][et_pb_text admin_label="Title and Subtitle" _builder_version="3.0.101" background_layout="light" module_alignment="center" module_class="lesson-summary text-single-column-narrow"]
<h1>JS Basics: Functions, Syntax, and Common Uses</h1>
<h2>A short intro to the core fundamentals of Javascript for front-end web development</h2>
[/et_pb_text][et_pb_post_title _builder_version="3.0.92" title="off" meta="on" author="on" date="off" categories="on" comments="off" featured_image="off" featured_placement="below" text_color="dark" text_background="off" module_class="lesson-summary text-single-column-narrow" /][et_pb_text admin_label="Introduction Summary and Outcomes" _builder_version="3.0.101" background_layout="light" module_class="lesson-summary text-single-column-narrow"]

Javascript (JS), often times referred to as "Vanilla JS," is used to added functionality to a web page (e.g. "do this when a user clicks this"). For many beginner web designers, JS can be daunting to learn. Many find JQuery to be much simpler and easier to use, learn, and implement. Knowing that JQuery is a JavaScript library that is based on JavaScript (that comes at the cost of adding it as a required dependency on page load), it makes sense to learn the source language first: JavaScript. Once you understand the basics of Vanilla JS, such as how to write a simple function, then the possibilities become endless. For example, if you can write a simple function that adds and removes a class on a HTML element (DOM manipulation) when a user clicks on something, then you can then manage the UX and control your UI via the HTML and CSS. This core front-end web development skill will enable you to do many, many, many things.
<blockquote>Alongside HTML and CSS, <strong>JavaScript</strong> is one of the three core technologies of World Wide Web content production.
<cite>– <a href="https://en.wikipedia.org/wiki/JavaScript">Wikipedia</a></cite></blockquote>
[/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row][et_pb_column type="4_4"][et_pb_text admin_label="Image + Caption" _builder_version="3.0.101" background_layout="light" text_orientation="center" module_alignment="center"]
<h4>The Anatomy of a JS Function</h4>
<img class="aligncenter size-full wp-image-1601" src="https://www.creativemedia.space/wp-content/uploads/2018/02/jsanatomy1-4x3.gif" alt="" width="1500" height="1000" />

[/et_pb_text][et_pb_text admin_label="Code Block" _builder_version="3.0.101" background_layout="light" module_class="text-single-column-narrow"]
<h3>Syntax for a Function Definition:</h3>
<pre><code>
function myFunctionName(optionalArguments) {
    var myVariableName = value;
    console.log(myVariableName); 
} 
</code></pre>
<h3>Syntax for a Function Call:</h3>
<pre><code>
functionName();
</code></pre>
[/et_pb_text][et_pb_text admin_label="Code Block" _builder_version="3.0.101" background_layout="light" module_class="text-single-column-narrow"]
<h3>Examples:</h3>
Using Vanilla JS, there are multiple ways to target elements via the DOM. One of the simplest ways to target a single, unique element (#id) is to use document.getElementById():
<pre><code>
    document.getElementById('mydiv')
</code></pre>
If you do not need to support older browsers, you can use querySelector or querySelectorAll, which will work with both id's and classes:
<pre><code>
    document.querySelector('#mydiv')
    document.querySelectorAll('.myclass')</code></pre>
Note: if there are multiple instances, such as multiple elements with the same class name, querySelector will only work on the first instance. If you need to target multiple instances of a class, then use querySelectorAll.
<h4>Linking to an external JS File</h4>
A recommended way to use JavaScript is to link to it in a separate file via a script tag. Just like HTML and CSS, JS has the same top-to-bottm running order, so when the browser encounters a block of JavaScript, it runs it in order, from top to bottom, all the way to the end, before it moves on. With that said, in most cases the html content is more important than the functionality (in other words, the functionality can come after the user sees the content), so for the reason, it is often times a best practice to place this JS code and linked script tags at the bottom of your html document, inside of your closing /body tag.
<h5>Inside your HTML file (at the bottom):</h5>
<pre><code>
&lt;script src="js/scripts.js"&gt;&lt;/script&gt;</code></pre>
<h5>In a separate JS file (e.g. script.js):;</h5>
<pre><code>
document.addEventListener('DOMContentLoaded', function() {

    var element = document.querySelector('#mydiv');
    element.addEventListener('click', function() {
      // do something
    });
    
})</code></pre>
<h3>JavaScript and the DOM (Document Object Model)</h3>
JS can store values (data), run operations on data (change data), listen to user actions (event listening), and make changes to elements within a html document directly in the browser immediately via DOM manipulation. The DOM API allows web developers to manipulate HTML and CSS, such as create, remove, and change HTML elements and dynamically apply new styles to elements on a web page. JS is natively supported by almost all browsers, which means that it is executed by the browser's JavaScript Engine (no plugin, server, or database required).
<h4>Example: Add/Remove a Class on a Single Element (e.g. on click event)</h4>
To target a single, unique element (class or id) using vanilla JS, you can use document.querySelector():
<pre><code>&lt;a href="#" class="mybutton"&gt;Unique Button&lt;/a&gt;

</code></pre>
You then need to add an event listener to handle a click event and a function to do something once an event is triggered.
<pre><code>
    document.querySelector('.mybutton').addEventListener('click', function(e) {
      this.classList.toggle('red');
      e.preventDefault();
    });

</code></pre>
<h4>Example: Add/Remove a Class on a Multiple Elements (e.g. on click event)</h4>
To target multiple elements (that share the same class) using vanilla JS, you can use document.querySelectorAll() and you'll need to loop through an array of elements:
<pre><code>
    &lt;a href="#" class="button"&gt;Regular Button&lt;/a&gt;
    &lt;a href="#" class="button"&gt;Regular Button&lt;/a&gt;
</code></pre>
<pre><code>
    var elements = document.querySelectorAll('.button');
    for ( var i = 0, len = elements.length; i &lt; len; i++ ) {
        elements[i].addEventListener('click', function(e) {
          this.classList.toggle('red');
          e.preventDefault();
        });
    }
</code></pre>
<h5>Notes:</h5>
<ul>
 	<li>document.querySelector('.classname') gets the first matching element</li>
 	<li>document.querySelectorAll('.classname') returns a node list of all matching elements.</li>
 	<li>These will only work on IE 9+. If you require support for older browsers, you can use a polyfill or use different methods, such as:
<ul>
 	<li><a href="https://github.com/eligrey/classList.js">Eli Grey's classList.js polyfill</a>. - works in all browsers IE8+</li>
 	<li>document.getElementById('#idname') - works in all browsers back to IE6+</li>
</ul>
</li>
</ul>
&nbsp;

[/et_pb_text][et_pb_text admin_label="Code Block" _builder_version="3.0.101" background_layout="light" module_class="text-single-column-narrow"]
<h3>JS Terminology</h3>
<em>A Brief Primer</em>
<h4>Variables</h4>
Variables are containers that you can store values in. You start by declaring a variable with the var keyword, followed by any name you want to call it:
<pre><code>
var myVariable;
myVariable = "Chris";
</code></pre>
<h4>Data Types</h4>
<ul>
 	<li>String</li>
 	<li>Number</li>
 	<li>Boolean</li>
 	<li>Array</li>
 	<li>Object</li>
</ul>
<h5>Arrays and Objects</h5>
An <strong>array</strong> is a collection of values are comma separated values

An <strong>object</strong> is a collection of both properties and values that are represented as key/value pairs, where each pair is separated by a comma.
<h4>Methods</h4>
<strong>Methods</strong> provide the ability to extend the power of an object by setting the value of a property to a function (e.g. the latter in an object's key/value pair).
<h4>Operators</h4>
An <strong>operator</strong> is a symbol which produces a result based on two values or variables.
<pre><code>
1 + 1 //here the + operator is used to add two numerical values
"Hello" + "Chris" //here the + operator is used to combine (concatenate) two values, or in this case: two strings.
</code></pre>
<h4>Conditionals</h4>
<pre><code>
if (something === true) {
    // do something
} else {
    // do something else
}
</code></pre>
<h4>Loops</h4>
<strong>Loops</strong> are used to repeat code multiple times, often used when you need to apply the same set of instructions to multiple elements on a web page. The basic anatomy of a loop is 1) a starting value (e.g. 1), and exit condition (e.g. when you get to the total number of instances of an element or class on a web page), and 3) an increment (+1 every time you go through the loop).

Here's an example of the syntax of a "for" loop:
<pre><code>
for (var i = 1 ; i &lt; totalnumberofitems ; i++) {
    // do something
    console.log(i)
}
</code></pre>
<h4>Dot Notation vs. Bracket Notation</h4>
<pre><code>
object.property;
object[property_name]
</code></pre>
<h4>Functions</h4>
A <strong>function</strong> is a sequence of instructions. You can think of them as "blocks" of code.
<h5>Function Definition and Call</h5>
A function is defined using the "function" keyword followed by a custom name and a set of parentheses (for any function arguments, if needed), then the "body" of the function is situated between two curly braces and can contain an unlimited number of statements, each of which must end with a semicolon.
<h4>Events</h4>
To add interactivity to a website using JS, you can use <strong>events</strong>. Events essentially "listen" for things to happen in the browser so that code can be triggered, or run, in response. A common example is the click event, that is executed ("fired" when a user clicks on something (or "touches" it via their device).

There are several different ways to attach an event to an element.
<pre><code>
document.querySelector('.myButton').onclick = function() {};
</code></pre>
<pre><code>
var myButton = document.querySelector('.myButtonClass');
myButton.onclick = function() {};
</code></pre>
<h3>Helpful Learning Resources:</h3>
<ul>
 	<li><a href="http://www.anatomyofcode.com/">Anatomy of Code</a></li>
</ul>
[/et_pb_text][/et_pb_column][/et_pb_row][/et_pb_section][et_pb_section bb_built="1" fullwidth="off" specialty="off" prev_background_color="#000000" next_background_color="#000000" _builder_version="3.0.101" custom_css_main_element="display: none;"][et_pb_row][et_pb_column type="4_4"][et_pb_text admin_label="Embedded Gist" _builder_version="3.0.92" background_layout="light" text_orientation="center" module_alignment="center"]
<h4>Blank web page linked to an external style.css file</h4>
[gist https://gist.github.com/kccnma/f1feca5a94fd9291214a497c68232e02 /]

[/et_pb_text][/et_pb_column][/et_pb_row][/et_pb_section][et_pb_section bb_built="1" fullwidth="off" specialty="off" prev_background_color="#000000" _builder_version="3.0.101" custom_css_main_element="display: none;"][et_pb_row][et_pb_column type="4_4"][et_pb_text admin_label="Conclusion" _builder_version="3.0.92" background_layout="light" module_class="text-single-column-narrow"]
<h2>Conclusion</h2>
CSS is fun and powerful. CSS files should be linked in the header and should include a commented table of contents at the top. Happy Styling!
<pre></pre>
[/et_pb_text][et_pb_text admin_label="Related Resources" _builder_version="3.0.92" background_layout="light" module_class="text-single-column-narrow"]
<h3>Related Resources and Reading</h3>
<ul>
 	<li>W3Schools Resources:
<ul>
 	<li><a href="https://www.w3schools.com/css/default.asp">CSS Tutorial</a></li>
 	<li><a href="https://www.w3schools.com/cssref/css_selectors.asp">CSS Selectors</a></li>
</ul>
</li>
 	<li>Chris Coyier's <a href="https://css-tricks.com/">CSS-Tricks.com</a></li>
 	<li>Adam Marsden’s <a href="https://adam-marsden.co.uk/css-cheat-sheet">CSS Cheat Sheet</a></li>
</ul>
<pre></pre>
[/et_pb_text][et_pb_text admin_label="Go Further" _builder_version="3.0.92" background_layout="light" module_class="text-single-column-narrow"]
<h3>Go Further</h3>
<ul>
 	<li>Read about <a href="https://en.wikipedia.org/wiki/Web_standards">Web Standards</a> and the <a href="https://www.w3.org/standards/">W3C</a> (World Wide Web Consortium).</li>
 	<li>Try coding a <a href="https://codepen.io/kccnma/pen/ppQdmo?editors=1100">simple HTML web page with base CSS</a>.</li>
</ul>
<pre></pre>
[/et_pb_text][et_pb_toggle admin_label="Author Notes" _builder_version="3.0.92" title="Author Notes" open="off" module_class="text-single-column-narrow"]
<h6>This was written specifically to help aspiring web designers as they aim to:</h6>
<ul>
 	<li>Learn the basic selectors, syntax, and common uses of CSS Styling</li>
</ul>
[/et_pb_toggle][/et_pb_column][/et_pb_row][/et_pb_section]