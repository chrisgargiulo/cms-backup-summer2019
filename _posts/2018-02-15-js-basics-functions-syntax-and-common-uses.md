---
ID: 1597
post_title: 'JS Basics: Functions and Syntax'
author: CMS
post_excerpt: ""
layout: post
permalink: >
  https://creativemedia.space/js-basics-functions-syntax-and-common-uses/
published: true
post_date: 2018-02-15 15:42:09
---
<!-- wp:heading {"level":3} -->
<h3>A short intro to the core fundamentals of Javascript for front-end web development</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Javascript (JS), often times referred to as "Vanilla JS," is used to added functionality to a web page (e.g. "do this when a user clicks this"). For many beginner web designers, JS can be daunting to learn. Many find JQuery to be much simpler and easier to use, learn, and implement. Knowing that JQuery is a JavaScript library that is based on JavaScript (that comes at the cost of adding it as a required dependency on page load), it makes sense to learn the source language first: JavaScript. Once you understand the basics of Vanilla JS, such as how to write a simple function, then the possibilities become endless. For example, if you can write a simple function that adds and removes a class on a HTML element (DOM manipulation) when a user clicks on something, then you can then manage the UX and control your UI via the HTML and CSS. This core front-end web development skill will enable you to do many, many, many things.</p>
<!-- /wp:paragraph -->

<!-- wp:quote -->
<blockquote class="wp-block-quote"><p>Alongside&nbsp;HTML&nbsp;and&nbsp;CSS, <strong>JavaScript</strong> is one of the three core technologies of&nbsp;World Wide Web&nbsp;content production.<br>– <a href="https://en.wikipedia.org/wiki/JavaScript">Wikipedia</a></p></blockquote>
<!-- /wp:quote -->

<!-- wp:heading {"level":4} -->
<h4>The Anatomy of a JS Function</h4>
<!-- /wp:heading -->

<!-- wp:image {"id":1601,"align":"center"} -->
<div class="wp-block-image"><figure class="aligncenter"><img src="http://egargiulo.com/cms/wp-content/uploads/2018/02/jsanatomy1-4x3.gif" alt="" class="wp-image-1601"/></figure></div>
<!-- /wp:image -->

<!-- wp:heading {"level":3} -->
<h3>Syntax for a Function Definition:</h3>
<!-- /wp:heading -->

<!-- wp:code -->
<pre class="wp-block-code"><code>
function myFunctionName(optionalArguments) {
    var myVariableName = value;
    console.log(myVariableName); 
} 
</code></pre>
<!-- /wp:code -->

<!-- wp:heading {"level":3} -->
<h3>Syntax for a Function Call:</h3>
<!-- /wp:heading -->

<!-- wp:code -->
<pre class="wp-block-code"><code>
functionName();
</code></pre>
<!-- /wp:code -->

<!-- wp:heading {"level":3} -->
<h3>Examples:</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Using Vanilla JS, there are multiple ways to target elements via the DOM. One of the simplest ways to target a single, unique element (#id) is to use document.getElementById():</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>
    document.getElementById('mydiv')
</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>If you do not need to support older browsers, you can use querySelector or querySelectorAll, which will work with both id's and classes:</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>
    document.querySelector('#mydiv')
    document.querySelectorAll('.myclass')</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Note: if there are multiple instances, such as multiple elements with the same class name, querySelector will only work on the first instance. If you need to target multiple instances of a class, then use querySelectorAll.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>Linking to an external JS File</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>A recommended way to use JavaScript is to link to it in a separate file via a script tag. Just like HTML and CSS, JS has the same top-to-bottom running order, so when the browser encounters a block of JavaScript, it runs it in order, from top to bottom, all the way to the end, before it moves on. With that said, in most cases the html content is more important than the functionality (in other words, the functionality can come after the user sees the content), so for the reason, it is often times a best practice to place this JS code and linked script tags at the bottom of your html document, inside of your closing /body tag.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":5} -->
<h5>Inside your HTML file (at the bottom):</h5>
<!-- /wp:heading -->

<!-- wp:code -->
<pre class="wp-block-code"><code>
&lt;script src="js/scripts.js">&lt;/script></code></pre>
<!-- /wp:code -->

<!-- wp:heading {"level":5} -->
<h5>In a separate JS file (e.g. script.js):;</h5>
<!-- /wp:heading -->

<!-- wp:code -->
<pre class="wp-block-code"><code>
document.addEventListener('DOMContentLoaded', function() {

    var element = document.querySelector('#mydiv');
    element.addEventListener('click', function() {
      // do something
    });
    
})</code></pre>
<!-- /wp:code -->

<!-- wp:heading {"level":3} -->
<h3>JavaScript and the DOM (Document Object Model)</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>JS can store values (data), run operations on data (change data), listen to user actions (event listening), and make changes to elements within a html document directly in the browser immediately via DOM manipulation. The DOM API allows web developers to manipulate HTML and CSS, such as create, remove, and change HTML elements and dynamically apply new styles to elements on a web page. JS is natively supported by almost all browsers, which means that it is executed by the browser's JavaScript Engine (no plugin, server, or database required).</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>Example: Add/Remove a Class on a Single Element (e.g. on click event)</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>To target a single, unique element (class or id) using vanilla JS, you can use document.querySelector():</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>&lt;a href="#" class="mybutton">Unique Button&lt;/a>

</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>You then need to add an event listener to handle a click event and a function to do something once an event is triggered.</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>
    document.querySelector('.mybutton').addEventListener('click', function(e) {
      this.classList.toggle('red');
      e.preventDefault();
    });

</code></pre>
<!-- /wp:code -->

<!-- wp:heading {"level":4} -->
<h4>Example: Add/Remove a Class on a Multiple Elements (e.g. on click event)</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>To target multiple elements (that share the same class) using vanilla JS, you can use document.querySelectorAll() and you'll need to loop through an array of elements:</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>
    &lt;a href="#" class="button">Regular Button&lt;/a>
    &lt;a href="#" class="button">Regular Button&lt;/a>
</code></pre>
<!-- /wp:code -->

<!-- wp:code -->
<pre class="wp-block-code"><code>
    var elements = document.querySelectorAll('.button');
    for ( var i = 0, len = elements.length; i &lt; len; i++ ) {
        elements[i].addEventListener('click', function(e) {
          this.classList.toggle('red');
          e.preventDefault();
        });
    }
</code></pre>
<!-- /wp:code -->

<!-- wp:heading {"level":5} -->
<h5>Notes:</h5>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li>document.querySelector('.classname') gets the first matching element</li><li>document.querySelectorAll('.classname') returns a node list of all matching elements.</li><li>These will only work on IE 9+. If you require support for older browsers, you can use a polyfill or use different methods, such as:
<ul><li><a href="https://github.com/eligrey/classList.js">Eli Grey's classList.js polyfill</a>. - works in all browsers IE8+</li><li>document.getElementById('#idname') - works in all browsers back to IE6+</li></ul>
</li></ul>
<!-- /wp:list -->

<!-- wp:heading {"level":3} -->
<h3>JS Terminology</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><em>A Brief Primer</em></p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>Variables</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Variables are containers that you can store values in. You start by declaring a variable with the var keyword, followed by any name you want to call it:</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>
var myVariable;
myVariable = "Chris";
</code></pre>
<!-- /wp:code -->

<!-- wp:heading {"level":4} -->
<h4>Data Types</h4>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li>String</li><li>Number</li><li>Boolean</li><li>Array</li><li>Object</li></ul>
<!-- /wp:list -->

<!-- wp:heading {"level":5} -->
<h5>Arrays and Objects</h5>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>An <strong>array</strong> is a collection of values are comma separated values</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>An <strong>object</strong> is a collection of both properties and values that are represented as key/value pairs, where each pair is separated by a comma.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>Methods</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Methods</strong> provide the ability to extend the power of an object by setting the value of a property to a function (e.g. the latter in an object's key/value pair).</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>Operators</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>An <strong>operator</strong> is a symbol which produces a result based on two values or variables.</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>
1 + 1 //here the + operator is used to add two numerical values
"Hello" + "Chris" //here the + operator is used to combine (concatenate) two values, or in this case: two strings.
</code></pre>
<!-- /wp:code -->

<!-- wp:heading {"level":4} -->
<h4>Conditionals</h4>
<!-- /wp:heading -->

<!-- wp:code -->
<pre class="wp-block-code"><code>
if (something === true) {
    // do something
} else {
    // do something else
}
</code></pre>
<!-- /wp:code -->

<!-- wp:heading {"level":4} -->
<h4>Loops</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><strong>Loops</strong> are used to repeat code multiple times, often used when you need to apply the same set of instructions to multiple elements on a web page. The basic anatomy of a loop is 1) a starting value (e.g. 1), and exit condition (e.g. when you get to the total number of instances of an element or class on a web page), and 3) an increment (+1 every time you go through the loop).</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Here's an example of the syntax of a "for" loop:</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>
for (var i = 1 ; i &lt; totalnumberofitems ; i++) {
    // do something
    console.log(i)
}
</code></pre>
<!-- /wp:code -->

<!-- wp:heading {"level":4} -->
<h4>Dot Notation vs. Bracket Notation</h4>
<!-- /wp:heading -->

<!-- wp:code -->
<pre class="wp-block-code"><code>
object.property;
object[property_name]
</code></pre>
<!-- /wp:code -->

<!-- wp:heading {"level":4} -->
<h4>Functions</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>A <strong>function</strong> is a sequence of instructions. You can think of them as "blocks" of code.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":5} -->
<h5>Function Definition and Call</h5>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>A function is defined using the "function" keyword followed by a custom name and a set of parentheses (for any function arguments, if needed), then the "body" of the function is situated between two curly braces and can contain an unlimited number of statements, each of which must end with a semicolon.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>Events</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>To add interactivity to a website using JS, you can use <strong>events</strong>. Events essentially "listen" for things to happen in the browser so that code can be triggered, or run, in response. A common example is the click event, that is executed ("fired" when a user clicks on something (or "touches" it via their device).</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>There are several different ways to attach an event to an element.</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>
document.querySelector('.myButton').onclick = function() {};
</code></pre>
<!-- /wp:code -->

<!-- wp:code -->
<pre class="wp-block-code"><code>
var myButton = document.querySelector('.myButtonClass');
myButton.onclick = function() {};
</code></pre>
<!-- /wp:code -->

<!-- wp:heading {"level":3} -->
<h3>Helpful Learning Resources:</h3>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li><a href="http://www.anatomyofcode.com/">Anatomy of Code</a></li></ul>
<!-- /wp:list -->

<!-- wp:heading -->
<h2>Conclusion</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Javascript is fun and powerful. External JS files should be linked via script in the bottom of the html document to avoid browser render-blocking. Happy Scripting!</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3>Related Resources and Reading</h3>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li>W3Schools Resources:
<ul><li><a href="https://www.w3schools.com/css/default.asp">JS Tutorial</a></li></ul>
</li><li>Wes Bos Resources:
<ul><li><a href="https://wesbos.com/courses/">Wes Bos's Online Courses</a></li><li><a href="https://javascript30.com/">Wes Bos's Javascript 30</a></li></ul>
</li></ul>
<!-- /wp:list -->

<!-- wp:heading {"level":3} -->
<h3>Go Further</h3>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li>Read about <a href="https://en.wikipedia.org/wiki/Web_standards">Web Standards</a> and the <a href="https://www.w3.org/standards/">W3C</a> (World Wide Web Consortium).</li></ul>
<!-- /wp:list -->

<!-- wp:heading {"level":3} -->
<h3>Author Notes</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>This was written specifically to help aspiring web designers as they aim to:</p>
<!-- /wp:paragraph -->

<!-- wp:list -->
<ul><li>Learn the basic syntax and common uses of Javascript for front-end web development.</li></ul>
<!-- /wp:list -->