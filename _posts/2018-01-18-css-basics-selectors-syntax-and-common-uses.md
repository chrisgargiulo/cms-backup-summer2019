---
ID: 1462
post_title: 'CSS Basics: Selectors and Syntax'
author: Sassy Sally
post_excerpt: ""
layout: post
permalink: >
  https://www.creativemedia.space/css-basics-selectors-syntax-and-common-uses/
published: true
post_date: 2018-01-18 10:12:36
---
[et_pb_section bb_built="1" fullwidth="off" specialty="off" next_background_color="#000000"][et_pb_row][et_pb_column type="4_4"][et_pb_image _builder_version="3.0.92" src="https://www.creativemedia.space/wp-content/uploads/2018/01/css-4x2.gif" show_in_lightbox="off" url_new_window="off" use_overlay="off" always_center_on_mobile="on" force_fullwidth="off" show_bottom_space="on" /][/et_pb_column][/et_pb_row][et_pb_row][et_pb_column type="4_4"][et_pb_text admin_label="Running Head" _builder_version="3.0.92" background_layout="light" module_class="articlerunninghead text-single-column-narrow"]

Lesson

[/et_pb_text][et_pb_text admin_label="Title and Subtitle" _builder_version="3.0.92" background_layout="light" module_alignment="center" module_class="lesson-summary text-single-column-narrow"]

<h1>CSS Basics: Selectors, Syntax, and Common Uses</h1>
<h2>A short intro to the core fundamentals of CSS as a styling language</h2>

[/et_pb_text][et_pb_post_title _builder_version="3.0.92" title="off" meta="on" author="on" date="off" categories="on" comments="off" featured_image="off" featured_placement="below" text_color="dark" text_background="off" module_class="lesson-summary text-single-column-narrow" /][et_pb_text admin_label="Introduction Summary and Outcomes" _builder_version="3.0.92" background_layout="light" module_class="lesson-summary text-single-column-narrow"]

CSS is a rapidly growing and evolving technology that keeps getting more powerful with each new feature that gets added to its <a href="https://www.w3.org/Style/CSS/specs.en.html">specifications</a>. For a "styling" language, it can do more than just affect the presentation of markup via the UI, it can also play an integral role in the overall user experience and add features and functionality to an end product.
<blockquote>Along with HTML and JavaScript, <strong>CSS </strong> is a cornerstone technology used by most websites to create visually engaging webpages, user interfaces for web applications, and user interfaces for many mobile applications.
<cite>– <a href="https://en.wikipedia.org/wiki/Cascading_Style_Sheets">Wikipedia</a></cite></blockquote>

[/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row][et_pb_column type="4_4"][et_pb_text admin_label="Image + Caption" _builder_version="3.0.92" background_layout="light" text_orientation="center" module_alignment="center"]

<h4>The Anatomy of a CSS Selector</h4>
<img class="aligncenter size-full wp-image-1467" src="https://www.creativemedia.space/wp-content/uploads/2018/01/css-selectoranatomy.gif" alt="" width="1500" height="1000" />

[/et_pb_text][et_pb_text admin_label="Code Block" _builder_version="3.0.92" background_layout="light" module_class="text-single-column-narrow"]

<pre><code>
selector {
    property: value;
}
</code></pre>

[/et_pb_text][/et_pb_column][/et_pb_row][/et_pb_section][et_pb_section bb_built="1" fullwidth="off" specialty="off" prev_background_color="#000000" next_background_color="#000000"][et_pb_row][et_pb_column type="4_4"][et_pb_text admin_label="Embedded Gist" _builder_version="3.0.92" background_layout="light" text_orientation="center" module_alignment="center"]

<h4>Blank web page linked to an external style.css file</h4>
[gist https://gist.github.com/kccnma/f1feca5a94fd9291214a497c68232e02 /]

[/et_pb_text][/et_pb_column][/et_pb_row][/et_pb_section][et_pb_section bb_built="1" fullwidth="off" specialty="off" prev_background_color="#000000" next_background_color="#000000"][et_pb_row][et_pb_column type="4_4"][et_pb_text admin_label="Embedded Gist" _builder_version="3.0.92" background_layout="light" text_orientation="center" module_alignment="center"]

<h4>Simple web page with basic typography styling via CSS</h4>

[/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row][et_pb_column type="1_2"][et_pb_text admin_label="Embedded Gist" _builder_version="3.0.92" background_layout="light" text_orientation="center" module_alignment="center"]

<h5>HTML</h5>
[gist https://gist.github.com/kccnma/8e23e593457c7bf9eea97f91e01e4c98 /]

[/et_pb_text][/et_pb_column][et_pb_column type="1_2"][et_pb_text admin_label="Embedded Gist" _builder_version="3.0.92" background_layout="light" text_orientation="center" module_alignment="center"]

<h4>CSS</h4>
[gist https://gist.github.com/kccnma/07c097807856b1aabad207bec6076389 /]

[/et_pb_text][/et_pb_column][/et_pb_row][/et_pb_section][et_pb_section bb_built="1" fullwidth="off" specialty="off" prev_background_color="#000000" next_background_color="#333333"][et_pb_row][et_pb_column type="4_4"][et_pb_text admin_label="Embedded CodePen" _builder_version="3.0.106" background_layout="light" text_orientation="center" module_alignment="center"]

<h4>Combined HTML + CSS Result</h4>
[codepen_embed height="600" theme_id="0" slug_hash="ppQdmo" default_tab="result" user="kccnma"]See the Pen <a href="https://codepen.io/kccnma/pen/ppQdmo/">Simple HTML Web Page with Base CSS (ART 128 Assignment #2)</a> by kccnma (<a href="https://codepen.io/kccnma">@kccnma</a>) on <a href="https://codepen.io">CodePen</a>.[/codepen_embed]

[/et_pb_text][/et_pb_column][/et_pb_row][/et_pb_section][et_pb_section bb_built="1" fullwidth="off" specialty="off" _builder_version="3.0.89" background_color="#333333" prev_background_color="#ffffff" next_background_color="#ffffff"][et_pb_row _builder_version="3.0.89"][et_pb_column type="1_4"][/et_pb_column][et_pb_column type="1_2"][et_pb_blurb admin_label="Quick Hands-on Exercise Blurb" _builder_version="3.0.92" title="Quick Hands-on Exercise" url_new_window="off" use_icon="on" font_icon="%%167%%" use_circle="off" use_circle_border="off" icon_placement="top" use_icon_font_size="off" background_layout="dark" icon_color="#ffffff" text_orientation="center" header_level="h2"]

Try to solve the challenge below by doing the following: in the first code example below, click on the "edit in codepen" button in the upper right, then add the appropriate HTML tags to the source text so that it renders the same as the second code example below.

[/et_pb_blurb][/et_pb_column][et_pb_column type="1_4"][/et_pb_column][/et_pb_row][et_pb_row][et_pb_column type="4_4"][et_pb_text admin_label="Embedded CodePen" _builder_version="3.0.89" background_layout="dark" text_orientation="center" module_alignment="center"]

<h4>Code Example of Text Without HTML Markup</h4>
[codepen_embed height="265" theme_id="0" slug_hash="OzpyLP" default_tab="html,result" user="kccnma"]See the Pen <a href="https://codepen.io/kccnma/pen/OzpyLP/">Intro to HTML Exercise</a> by kccnma (<a href="https://codepen.io/kccnma">@kccnma</a>) on <a href="https://codepen.io">CodePen</a>.[/codepen_embed]

Note how the browser ignores line breaks.

[/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row][et_pb_column type="4_4"][et_pb_text admin_label="Embedded CodePen" _builder_version="3.0.106" background_layout="dark" text_orientation="center" module_alignment="center"]

<h4>Code Example of Text With HTML Markup</h4>
[codepen_embed height="265" theme_id="0" slug_hash="XVMXJQ" default_tab="html,result" user="kccnma"]See the Pen <a href="https://codepen.io/kccnma/pen/XVMXJQ/">Intro to HTML Exercise - with HTML Markup</a> by kccnma (<a href="https://codepen.io/kccnma">@kccnma</a>) on <a href="https://codepen.io">CodePen</a>.[/codepen_embed]

Note how the browser has default styling for each element.

[/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row][et_pb_column type="4_4"][et_pb_text admin_label="Embedded CodePen" _builder_version="3.0.106" background_layout="dark" text_orientation="center" module_alignment="center"]

<h4>Code Example of Text With HTML Markup + CSS</h4>
[codepen_embed height="265" theme_id="0" slug_hash="ppQdmo" default_tab="css,result" user="kccnma"]See the Pen <a href="https://codepen.io/kccnma/pen/ppQdmo/">Simple HTML Web Page with Base CSS (ART 128 Assignment #2)</a> by kccnma (<a href="https://codepen.io/kccnma">@kccnma</a>) on <a href="https://codepen.io">CodePen</a>.[/codepen_embed]

[/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row _builder_version="3.0.89"][et_pb_column type="1_4"][/et_pb_column][et_pb_column type="1_2"][et_pb_blurb admin_label="Quick Hands-on Exercise Blurb" _builder_version="3.0.92" title="Good Job!" url_new_window="off" use_icon="on" font_icon="%%277%%" use_circle="off" use_circle_border="off" icon_placement="top" use_icon_font_size="on" background_layout="dark" icon_color="#ffffff" text_orientation="center" icon_font_size="32px"]

If you completed this exercise, nice work! Coding isn't so bad is it?

[/et_pb_blurb][/et_pb_column][et_pb_column type="1_4"][/et_pb_column][/et_pb_row][/et_pb_section][et_pb_section bb_built="1" fullwidth="off" specialty="off" prev_background_color="#333333"][et_pb_row][et_pb_column type="4_4"][et_pb_text admin_label="Conclusion" _builder_version="3.0.92" background_layout="light" module_class="text-single-column-narrow"]

<h2>Conclusion</h2>
CSS is fun and powerful. CSS files should be linked in the header and should include a commented table of contents at the top. Happy Styling!
<pre>
</pre>

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
<pre>
</pre>

[/et_pb_text][et_pb_toggle admin_label="Author Notes" _builder_version="3.0.92" title="Author Notes" open="off" module_class="text-single-column-narrow"]

<h6>This was written specifically to help aspiring web designers as they aim to:</h6>
<ul>
 	<li>Learn the basic selectors, syntax, and common uses of CSS Styling</li>
</ul>

[/et_pb_toggle][/et_pb_column][/et_pb_row][/et_pb_section]