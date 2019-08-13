---
ID: 1462
post_title: 'CSS Basics: Selectors and Syntax'
author: CMS
post_excerpt: ""
layout: post
permalink: >
  https://creativemedia.space/css-basics-selectors-syntax-and-common-uses/
published: true
post_date: 2018-01-18 10:12:36
---
<!-- wp:heading {"level":3} -->
<h3>A short intro to the core fundamentals of CSS as a styling language</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>CSS is a rapidly growing and evolving technology that keeps getting more powerful with each new feature that gets added to its <a href="https://www.w3.org/Style/CSS/specs.en.html">specifications</a>. For a "styling" language, it can do more than just affect the presentation of markup via the UI, it can also play an integral role in the overall user experience and add features and functionality to an end product.</p>
<!-- /wp:paragraph -->

<!-- wp:more -->
<!--more-->
<!-- /wp:more -->

<!-- wp:quote -->
<blockquote class="wp-block-quote"><p>Along with HTML and JavaScript, <strong>CSS </strong> is a cornerstone technology used by most websites to create visually engaging webpages, user interfaces for web applications, and user interfaces for many mobile applications.<br />– <a href="https://en.wikipedia.org/wiki/Cascading_Style_Sheets">Wikipedia</a></p></blockquote>
<!-- /wp:quote -->

<!-- wp:heading {"level":4} -->
<h4>The Anatomy of a CSS Selector</h4>
<!-- /wp:heading -->

<!-- wp:image {"align":"center","id":1467} -->
<div class="wp-block-image"><figure class="aligncenter"><img src="http://egargiulo.com/cms/wp-content/uploads/2018/01/css-selectoranatomy.gif" alt="" class="wp-image-1467"/></figure></div>
<!-- /wp:image -->

<!-- wp:code -->
<pre class="wp-block-code"><code>
selector {
    property: value;
}
</code></pre>
<!-- /wp:code -->

<!-- wp:separator -->
<hr class="wp-block-separator"/>
<!-- /wp:separator -->

<!-- wp:heading {"level":4} -->
<h4>Blank web page linked to an external style.css file</h4>
<!-- /wp:heading -->

<!-- wp:shortcode -->
[gist https://gist.github.com/kccnma/f1feca5a94fd9291214a497c68232e02 /]
<!-- /wp:shortcode -->

<!-- wp:heading {"level":3} -->
<h3>Simple web page with basic typography styling via CSS </h3>
<!-- /wp:heading -->

<!-- wp:heading {"level":4} -->
<h4>HTML</h4>
<!-- /wp:heading -->

<!-- wp:shortcode -->
[gist https://gist.github.com/kccnma/8e23e593457c7bf9eea97f91e01e4c98 /]
<!-- /wp:shortcode -->

<!-- wp:heading {"level":4} -->
<h4>CSS</h4>
<!-- /wp:heading -->

<!-- wp:shortcode -->
[gist https://gist.github.com/kccnma/07c097807856b1aabad207bec6076389 /]
<!-- /wp:shortcode -->

<!-- wp:heading {"level":4} -->
<h4>Combined HTML + CSS Result</h4>
<!-- /wp:heading -->

<!-- wp:shortcode -->
[codepen_embed height="600" theme_id="0" slug_hash="ppQdmo" default_tab="result" user="kccnma"]See the Pen <a href="https://codepen.io/kccnma/pen/ppQdmo/">Simple HTML Web Page with Base CSS (ART 128 Assignment #2)</a> by kccnma (<a href="https://codepen.io/kccnma">@kccnma</a>) on <a href="https://codepen.io">CodePen</a>.[/codepen_embed]
<!-- /wp:shortcode -->

<!-- wp:separator -->
<hr class="wp-block-separator"/>
<!-- /wp:separator -->

<!-- wp:heading -->
<h2><strong>Quick</strong> Hands-on Exercise</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Try to solve the challenge below by doing the following: in the first code example below, click on the "edit in codepen" button in the upper right, then add the appropriate HTML tags to the source text so that it renders the same as the second code example below.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>Code Example of Text Without HTML Markup</h4>
<!-- /wp:heading -->

<!-- wp:shortcode -->
[codepen_embed height="265" theme_id="0" slug_hash="OzpyLP" default_tab="html,result" user="kccnma"]See the Pen <a href="https://codepen.io/kccnma/pen/OzpyLP/">Intro to HTML Exercise</a> by kccnma (<a href="https://codepen.io/kccnma">@kccnma</a>) on <a href="https://codepen.io">CodePen</a>.[/codepen_embed]
<!-- /wp:shortcode -->

<!-- wp:paragraph -->
<p>Note how the browser ignores line breaks.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>Code Example of Text With HTML Markup</h4>
<!-- /wp:heading -->

<!-- wp:shortcode -->
[codepen_embed height="265" theme_id="0" slug_hash="XVMXJQ" default_tab="html,result" user="kccnma"]See the Pen <a href="https://codepen.io/kccnma/pen/XVMXJQ/">Intro to HTML Exercise - with HTML Markup</a> by kccnma (<a href="https://codepen.io/kccnma">@kccnma</a>) on <a href="https://codepen.io">CodePen</a>.[/codepen_embed]
<!-- /wp:shortcode -->

<!-- wp:paragraph -->
<p>Note how the browser has default styling for each element.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>Code Example of Text With HTML Markup + CSS</h4>
<!-- /wp:heading -->

<!-- wp:shortcode -->
[codepen_embed height="265" theme_id="0" slug_hash="ppQdmo" default_tab="css,result" user="kccnma"]See the Pen <a href="https://codepen.io/kccnma/pen/ppQdmo/">Simple HTML Web Page with Base CSS (ART 128 Assignment #2)</a> by kccnma (<a href="https://codepen.io/kccnma">@kccnma</a>) on <a href="https://codepen.io">CodePen</a>.[/codepen_embed]
<!-- /wp:shortcode -->

<!-- wp:heading {"level":4} -->
<h4>Good Job!</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>If you completed this exercise, nice work! Coding isn't so bad is it?</p>
<!-- /wp:paragraph -->

<!-- wp:separator -->
<hr class="wp-block-separator"/>
<!-- /wp:separator -->

<!-- wp:heading -->
<h2>Conclusion</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>CSS is fun and powerful. CSS files should be linked in the header and should include a commented table of contents at the top. Happy Styling!</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3>Related Resources and Reading</h3>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li>W3Schools Resources:
<ul><li><a href="https://www.w3schools.com/css/default.asp">CSS Tutorial</a></li><li><a href="https://www.w3schools.com/cssref/css_selectors.asp">CSS Selectors</a></li></ul>
</li><li>Chris Coyier's <a href="https://css-tricks.com/">CSS-Tricks.com</a></li><li>Adam Marsden’s <a href="https://adam-marsden.co.uk/css-cheat-sheet">CSS Cheat Sheet</a></li></ul>
<!-- /wp:list -->

<!-- wp:heading {"level":3} -->
<h3>Go Further</h3>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li>Read about <a href="https://en.wikipedia.org/wiki/Web_standards">Web Standards</a> and the <a href="https://www.w3.org/standards/">W3C</a> (World Wide Web Consortium).</li><li>Try coding a <a href="https://codepen.io/kccnma/pen/ppQdmo?editors=1100">simple HTML web page with base CSS</a>.</li></ul>
<!-- /wp:list -->

<!-- wp:separator -->
<hr class="wp-block-separator"/>
<!-- /wp:separator -->

<!-- wp:heading {"level":3} -->
<h3>Author Notes</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>This was written specifically to help aspiring web designers as they aim to:</p>
<!-- /wp:paragraph -->

<!-- wp:list -->
<ul><li>Learn the basic selectors, syntax, and common uses of CSS Styling</li></ul>
<!-- /wp:list -->

<!-- wp:paragraph -->
<p></p>
<!-- /wp:paragraph -->