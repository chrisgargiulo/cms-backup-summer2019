---
ID: 1612
post_title: Create a Simple Portfolio Site
author: CMS
post_excerpt: ""
layout: post
permalink: >
  https://creativemedia.space/simple-portfolio-site/
published: true
post_date: 2018-02-22 17:50:05
---
<!-- wp:heading -->
<h2>Display your work by coding an online portfolio site from&nbsp;scratch</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>There are many different ways to share your work online. If you are a web designer with front-end web development skills looking to showcase your talent, one of the best ways is to custom design and code your own portfolio site from scratch.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>See a Demo<br><a href="http://nma.kcc.hawaii.edu/gargiulo/tests/portfolios/customportfolio1/">http://nma.kcc.hawaii.edu/gargiulo/tests/portfolios/customportfolio1/</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>View on Github<br><a href="https://github.com/kccnma/teachingmaterials/tree/master/customportfolio1">https://github.com/kccnma/teachingmaterials/tree/master/customportfolio1</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>View on Codepen<br><a href="https://codepen.io/kccnma/pen/bLKKqV">https://codepen.io/kccnma/pen/bLKKqV</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Download Starter Files<br><a href="http://nma.kcc.hawaii.edu/gargiulo/tests/portfolios/img.zip">http://nma.kcc.hawaii.edu/gargiulo/tests/portfolios/img.zip</a></p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2>Let's Code!</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><em>Get started by launching your favorite code editor (IDE)</em></p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>Create a new HTML folder named "customportfolio"</h4>
<!-- /wp:heading -->

<!-- wp:image {"id":1619,"align":"center"} -->
<div class="wp-block-image"><figure class="aligncenter"><img src="http://egargiulo.com/cms/wp-content/uploads/2018/02/cp1-folder-initialsetup.png" alt="" class="wp-image-1619"/></figure></div>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Inside of your new directory, create a new <strong>index.html</strong> file and then <a href="http://nma.kcc.hawaii.edu/gargiulo/tests/portfolios/img.zip">download the provided portfolio images for this exercise</a>.&nbsp; Next, create another new folder named "css" and inside of it create a new file named <strong>style.css</strong>. These two files (<em>index.html</em> and <em>style.css</em>) are the initial files that we will be editing. Once you are all setup, your local folder setup should look something like this:<br>Code, Save, Refresh, Repeat!</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>Start with Markup (HTML), then add Styling (CSS), then Repeat.</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Ideally, you should code line-by-line and write every line of html and css from the source code below <em>by hand</em>. To speed up the process (for those with neither the time or patience), please feel free to copy-and-paste large blocks of code, one-at-a-time, in order. After each iteration (code block), be sure to hit <em>save</em> then <em>preview</em> your changes in the browser (<em>refresh</em>) before moving on the the next code block.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":5} -->
<h5>HTML</h5>
<!-- /wp:heading -->

<!-- wp:shortcode -->
[gist https://gist.github.com/kccnma/0857a371f00861d41a1eb51a540a02d8 /]
<!-- /wp:shortcode -->

<!-- wp:paragraph -->
<p>...and also start with an empty style.css file with the following table of contents.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":5} -->
<h5>CSS</h5>
<!-- /wp:heading -->

<!-- wp:shortcode -->
[gist https://gist.github.com/kccnma/3cf6e89485eb1ebc5c7ad62b96348ac5/]
<!-- /wp:shortcode -->

<!-- wp:paragraph -->
<p>Then add the following body contents:</p>
<!-- /wp:paragraph -->

<!-- wp:list -->
<ul><li>header
<ul><li>navigation</li></ul>
</li><li>main
<ul><li>one section with a bunch of images</li></ul>
</li><li>footer
<ul><li>navigation</li></ul>
</li></ul>
<!-- /wp:list -->

<!-- wp:heading {"level":5} -->
<h5>HTML</h5>
<!-- /wp:heading -->

<!-- wp:shortcode -->
[gist https://gist.github.com/kccnma/70f8c36a2fbe8c8191c23701b20dd11f/]
<!-- /wp:shortcode -->

<!-- wp:paragraph -->
<p>Add in your HTML5 css (for IE8 and below) along with the least amount of main body and typography styling.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Notice how there is no css reset, nor a comprehensive typography setup. This minimal approach to custom (bespoke) development keeps your code lean by embracing browser defaults.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":5} -->
<h5>CSS</h5>
<!-- /wp:heading -->

<!-- wp:shortcode -->
[gist https://gist.github.com/kccnma/498a473b872c07d584191e6745b404ff/]
<!-- /wp:shortcode -->

<!-- wp:paragraph -->
<p>Next add your structural css for your site header, nav, and footer.<br><br></p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":5} -->
<h5>CSS</h5>
<!-- /wp:heading -->

<!-- wp:shortcode -->
[gist https://gist.github.com/kccnma/6da79245b1b6fbe9f7a0b61c7baf2fdf/]
<!-- /wp:shortcode -->

<!-- wp:paragraph -->
<p>Next, lets code a simple image grid from scratch, only instead of reverting to your safe go-to methods (e.g. inline-blocks or floated elements), you should try to be a little more <em>flexible</em> and use flex-box!</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":5} -->
<h5>CSS</h5>
<!-- /wp:heading -->

<!-- wp:shortcode -->
[gist https://gist.github.com/kccnma/f0300750da15e82a86c0f6d752c58f64/]
<!-- /wp:shortcode -->

<!-- wp:paragraph -->
<p>Once the home page is stable, let's create the two main sub pages:</p>
<!-- /wp:paragraph -->

<!-- wp:list -->
<ul><li>about.html</li><li>contact.html</li></ul>
<!-- /wp:list -->

<!-- wp:paragraph -->
<p>The header and footer are the same (except for the "selected" state (class) on the nav, so simply do a save-as from your index.html, update your title tag, move your selected state to the correct nav item, and lastly, add the body content alone.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":5} -->
<h5>HTML</h5>
<!-- /wp:heading -->

<!-- wp:shortcode -->
[gist https://gist.github.com/kccnma/4d57afcdd613668d234000b8cd2da02c/]
<!-- /wp:shortcode -->

<!-- wp:shortcode -->
[gist https://gist.github.com/kccnma/a931678a8f75e516497cf83f08ded13e/]
<!-- /wp:shortcode -->

<!-- wp:paragraph -->
<p>Once the primary sub pages are set up and working OK, let's create one portfolio entry sub page using the "web site" project as our working example content.<br><br></p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":5} -->
<h5>HTML</h5>
<!-- /wp:heading -->

<!-- wp:shortcode -->
[gist https://gist.github.com/kccnma/98cc9374a1a618254205488210d636cc/]
<!-- /wp:shortcode -->

<!-- wp:paragraph -->
<p>For the sub pages, we're going to need some css help for the hero section (to break out of our fixed-width and go full-width) and for our internal content layout, which we'll use a traditional layout grid, only this time, let's use flexbox!</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":5} -->
<h5>CSS</h5>
<!-- /wp:heading -->

<!-- wp:shortcode -->
[gist https://gist.github.com/kccnma/c7ea7c757c47353e0bc1a3f2723e4894/]
<!-- /wp:shortcode -->

<!-- wp:heading {"level":3} -->
<h3>Let's Spice it Up!</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Finally, lets add some simple (fake) page transitions that with a "fade-in" and "move-in" effect via css3 animation.<br><br></p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":5} -->
<h5>CSS</h5>
<!-- /wp:heading -->

<!-- wp:shortcode -->
[gist https://gist.github.com/kccnma/a3744153228ecf5ecd1ce240e3909bfa/]
<!-- /wp:shortcode -->

<!-- wp:paragraph -->
<p></p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>When you are done, the home page should look like this:</h4>
<!-- /wp:heading -->

<!-- wp:shortcode -->
[codepen_embed height="660" theme_id="0" slug_hash="bLKKqV" default_tab="result" user="kccnma"]See the Pen <a href="https://codepen.io/kccnma/pen/bLKKqV/">Custom Portfolio Test #0.1</a> by kccnma (<a href="https://codepen.io/kccnma">@kccnma</a>) on <a href="https://codepen.io">CodePen</a>.[/codepen_embed]
<!-- /wp:shortcode -->

<!-- wp:paragraph -->
<p>For the completed version with sub pages and additional css (e.g. circular image helper), see the demo and source code via the links below:</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>See a Demo<br><a href="http://nma.kcc.hawaii.edu/gargiulo/tests/portfolios/customportfolio1/">http://nma.kcc.hawaii.edu/gargiulo/tests/portfolios/customportfolio1/</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>View on Github Button<br><a href="https://github.com/kccnma/teachingmaterials/tree/master/customportfolio1">https://github.com/kccnma/teachingmaterials/tree/master/customportfolio1</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>View on Codepen<br><a href="https://codepen.io/kccnma/pen/bLKKqV">https://codepen.io/kccnma/pen/bLKKqV</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Download Starter Files<br><a href="http://nma.kcc.hawaii.edu/gargiulo/tests/portfolios/img.zip">http://nma.kcc.hawaii.edu/gargiulo/tests/portfolios/img.zip</a></p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>Next Steps: Continue adding more pages with real content</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>After the home page is secure, along with at least one project/portfolio entry sub page, you can move on to add all pages with real content. As you add all sub pages and content, be sure to test on multiple devices and screen sizes and try designing-as-you-code. You might find it helpful (and easier at times) to design in the browser instead of in your usual design application.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>One last thing: Have fun!</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2>Summary</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Coding your online portfolio is never an easy task. There are so many ways to present your work, so which way is best? Unfortunately there is no right or wrong answer—only you can make this decision. The good news is that you can use your online portfolio as a great excuse to practice writing custom hand-written code from scratch, because the best way to become a stronger web designer and front-end web developer is <strong>to create web sites</strong>.&nbsp; The the more custom coded sites you make, the easier it will get as you develop your own best practices for writing code and solving code-related UX and UI problems.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3>Related Resources and Reading</h3>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li>Chris's <a href="http://nma.kcc.hawaii.edu/gargiulo/blog/portfolioentry.html">Blog post on Portfolio Entries</a></li><li>Chris's <a href="http://nma.kcc.hawaii.edu/gargiulo/tests/portfolios/">various portfolio tests</a></li></ul>
<!-- /wp:list -->

<!-- wp:heading {"level":3} -->
<h3>Go Further</h3>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li>Explore and test out different custom grid layouts like <a href="http://nma.kcc.hawaii.edu/gargiulo/blog/images/portfolioexamples/grids/mockupgrid-variablesizes.html">this mockup grid test with variable-sized thumb images</a>.</li><li>Consider implementing a sortable gallery
<ul><li>Check out <a href="https://www.kunkalabs.com/mixitup/">MixItUp by Kunk Labs</a></li></ul>
</li></ul>
<!-- /wp:list -->

<!-- wp:heading {"level":3} -->
<h3>Author Notes</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>This was written specifically to help aspiring web designers as they aim to:</p>
<!-- /wp:paragraph -->

<!-- wp:list -->
<ul><li>Synthesize the concepts and skills garnered as a designer and front-end web developer by showcasing a culmination of projects in a custom designed and coded bespoke interface that integrates conceptual thinking and aesthetic application.</li></ul>
<!-- /wp:list -->