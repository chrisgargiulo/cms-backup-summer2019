---
ID: 2211
post_title: Positioning and Layout Tests
author: CMS
post_excerpt: ""
layout: post
permalink: >
  https://creativemedia.space/exercise-positioning-layout-tests/
published: true
post_date: 2019-02-12 14:43:03
---
<!-- wp:heading {"level":3} -->
<h3>Hands-on exercises to help understand different layout techniques</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Check out the codepen examples below, each with multiple ways to center content. Be sure to delete the css (or comment it out) line-by-line so you can fully understand the impact of each css property and value.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3>Centering</h3>
<!-- /wp:heading -->

<!-- wp:heading {"level":4} -->
<h4>Horizontal Centering</h4>
<!-- /wp:heading -->

<!-- wp:shortcode -->
[codepen_embed height="500" theme_id="0" slug_hash="xMjyZK" default_tab="css,result" user="kccnma"]See the Pen <a href="https://codepen.io/kccnma/pen/xMjyZK/">Exercise: Simple Horizontal Centering</a> by kccnma (<a href="https://codepen.io/kccnma">@kccnma</a>) on <a href="https://codepen.io">CodePen</a>.[/codepen_embed]
<!-- /wp:shortcode -->

<!-- wp:paragraph -->
<p>Note how it's just one line of code: text-align: center;</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>Horizontal + Vertical Centering</h4>
<!-- /wp:heading -->

<!-- wp:shortcode -->
[codepen_embed height="500" theme_id="0" slug_hash="mvLzBw" default_tab="css,result" user="kccnma"]See the Pen <a href="https://codepen.io/kccnma/pen/mvLzBw/">Exercise: Simple Horizontal and Vertical Centering with Flexbox</a> by kccnma (<a href="https://codepen.io/kccnma">@kccnma</a>) on <a href="https://codepen.io">CodePen</a>.[/codepen_embed]
<!-- /wp:shortcode -->

<!-- wp:paragraph -->
<p>Note the use of flexbox and subsequent two (three total) lines of code: display: flex; justify-content: center; align-items: center;</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3>Absolute vs. Relative Positioning</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Understanding when to use each is important and empowering.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>HINT: it's all about preserving normal flow.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>"Don't break me."&nbsp;–Normal Flow</h4>
<!-- /wp:heading -->

<!-- wp:shortcode -->
[codepen_embed height="500" theme_id="0" slug_hash="ddyQEZ" default_tab="css,result" user="kccnma"]See the Pen <a href="https://codepen.io/kccnma/pen/ddyQEZ/">CSS Positioning Test #1: Absolute vs. Relative</a> by kccnma (<a href="https://codepen.io/kccnma">@kccnma</a>) on <a href="https://codepen.io">CodePen</a>.[/codepen_embed]
<!-- /wp:shortcode -->

<!-- wp:paragraph -->
<p>Note how absolute positioning breaks normal flow.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>It's all Relative...</h4>
<!-- /wp:heading -->

<!-- wp:shortcode -->
[codepen_embed height="500" theme_id="0" slug_hash="NyWepK" default_tab="css,result" user="kccnma"]See the Pen <a href="https://codepen.io/kccnma/pen/NyWepK/">CSS Position Test #2: Absolute child inside of a Relative Parent</a> by kccnma (<a href="https://codepen.io/kccnma">@kccnma</a>) on <a href="https://codepen.io">CodePen</a>.[/codepen_embed]
<!-- /wp:shortcode -->

<!-- wp:paragraph -->
<p>HINT: when you think of the word "relative" try to think of a family member such as your parent. In this context, whenever you are positioning an element using absolute positioning, think of it like a child and ask "who is the parent?" When a parent gets a position: relative setting, it becomes the 0,0 (x,y) coordinate for it's absolutely positioned children.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3>Floats vs. Inline-Blocks</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>When it comes to two-dimensional content, such as a grid of thumb images, flexbox is now well supported in all modern browsers so it is highly recommended, but I also recommend understanding the strategies behind two old-school, tried-and-true techniques (and their shortcomings): 1) Floats (including the need for "clearing" floats with "clear fixes" and 2) inline-blocks (and the inline "space" between them):</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>Floats</h4>
<!-- /wp:heading -->

<!-- wp:shortcode -->
[codepen_embed height="500" theme_id="0" slug_hash="mXdoPw" default_tab="css,result" user="kccnma"]See the Pen <a href="https://codepen.io/kccnma/pen/mXdoPw/">CSS Positioning Test #3: Floats</a> by kccnma (<a href="https://codepen.io/kccnma">@kccnma</a>) on <a href="https://codepen.io">CodePen</a>.[/codepen_embed]
<!-- /wp:shortcode -->

<!-- wp:paragraph -->
<p>Note the "clearfix" css used to keep the parent element open</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>Inline Blocks</h4>
<!-- /wp:heading -->

<!-- wp:shortcode -->
[codepen_embed height="500" theme_id="0" slug_hash="KQKEzr" default_tab="css,result" user="kccnma"]See the Pen <a href="https://codepen.io/kccnma/pen/KQKEzr/">CSS Positioning Test #4: Inline-Block</a> by kccnma (<a href="https://codepen.io/kccnma">@kccnma</a>) on <a href="https://codepen.io">CodePen</a>.[/codepen_embed]
<!-- /wp:shortcode -->

<!-- wp:paragraph -->
<p>Note the space between each inline-block element</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3>Custom Grid Systems</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Custom semantic grids are super helpful and convenient when laying out content. There&nbsp; are multiple ways to code your own grid from scratch (it's not that hard to do and takes very little time), such as using floats, flexbox, and CSS&nbsp;Grid. Each has it's own challenges and advantages, so it's helpful to understand the proc and cons for each. Here's a simple flexbox grid with useful semantic classnames and helper utility classes that can be easily used (and reused) for many common layout scenarios:</p>
<!-- /wp:paragraph -->

<!-- wp:shortcode -->
[codepen_embed height="1000" theme_id="0" slug_hash="NORrOp" default_tab="result" user="kccnma"]See the Pen <a href="https://codepen.io/kccnma/pen/NORrOp/">Reusable Semantic Grid System for Page Layout: Using Flexbox</a> by kccnma (<a href="https://codepen.io/kccnma">@kccnma</a>) on <a href="https://codepen.io">CodePen</a>.[/codepen_embed]
<!-- /wp:shortcode -->

<!-- wp:paragraph -->
<p>If you completed these exercises, nice work!</p>
<!-- /wp:paragraph -->