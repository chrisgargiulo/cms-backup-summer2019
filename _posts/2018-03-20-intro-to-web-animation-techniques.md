---
ID: 1700
post_title: Intro to Web Animation Techniques
author: Front-end Freddy
post_excerpt: ""
layout: post
permalink: >
  https://www.creativemedia.space/intro-to-web-animation-techniques/
published: true
post_date: 2018-03-20 17:49:06
---
[et_pb_section bb_built="1" fullwidth="off" specialty="off" _builder_version="3.0.89" next_background_color="#000000"][et_pb_row][et_pb_column type="4_4"][et_pb_image _builder_version="3.0.101" src="https://www.creativemedia.space/wp-content/uploads/2018/03/webanimation-4x2.gif" show_in_lightbox="off" url_new_window="off" use_overlay="off" always_center_on_mobile="on" force_fullwidth="off" show_bottom_space="on" /][/et_pb_column][/et_pb_row][et_pb_row _builder_version="3.0.89"][et_pb_column type="4_4"][et_pb_text admin_label="Running Head" _builder_version="3.0.101" background_layout="light" module_class="articlerunninghead text-single-column-narrow"]

Lesson

[/et_pb_text][et_pb_text admin_label="Title and Subtitle" _builder_version="3.0.101" background_layout="light" module_alignment="center" module_class="lesson-summary text-single-column-narrow"]
<h1>Introduction to Web Animation Techniques and Technologies</h1>
<h2>CSS, JS, Animated Gifs, Videos, SVG, and More...</h2>
[/et_pb_text][et_pb_post_title _builder_version="3.0.89" title="off" meta="on" author="on" date="off" categories="off" comments="off" featured_image="off" featured_placement="below" text_color="dark" text_background="off" module_class="lesson-summary text-single-column-narrow" /][et_pb_text admin_label="Summary Text - Single Column Narrow" _builder_version="3.0.101" background_layout="light" module_class="text-single-column-narrow" saved_tabs="all"]
<blockquote>Purposeful animation can be used to guide users through a workflow in the same way that good typography should underscore the hierarchy of information in a document.
<cite> – Rachel Nabors, Web Animation Engineer</cite></blockquote>
Ever since Apple choose to not support the Flash player on the iPhone, thus ending Flash's reign as the de facto standard for animation on the web, web designers were forced to rethink the role of web animation during this transitional period while trying to figure out and make sense of the many different web animation approaches and technologies over the years. Thanks to the increasing browser support of CSS3 Animation (in combination with good ole' Javascript), web animation has made a comeback and has evolved with many new and exciting technologies and emerging solutions. Sadly, there is still no home-run "one-size-fits-all" GUI solution like Flash (web designers can't simply open up Flash, throw some keyframes on a timeline, and hit enter), but the good news is that web designers can animate using code. And it's not that hard to do once you get the basics. Let's dive in...
<h2>A Quick Overview</h2>
There are several different ways to animate on the web, with CSS and JS being the predominant two front-end technologies. Before discussing the current state of technologies and techniques, it is important to note that there are several different contexts and new applications for animation on the web today that go beyond the traditional non-interactive narrative animations (e.g. promotional videos and animated illustrations). For example, web animation is being used to create highly interactive and visually complex interfaces and systems (e.g. games, hybrid apps, "rich" web sites with animated page transitions, scroll-triggered animations, etc.). Lastly, we are seeing an increasing use of smaller, more subtle UI animations (e.g. animated menus and animated UI components) where web animation is used for improved usability and UX.

Given the above stated technologies and contexts, here are a few general guidelines to consider:
<ul>
 	<li><em>For subtle UI based web animation</em>, use CSS3 animation. If user interactivity is required, add in a light amount of Javascript for DOM manipulation (e.g. toggle class on user click).</li>
 	<li><em>For more complex UI web animations</em>, such as scroll-triggered animations and animated page transitions, you'll need to use Javascript. Your JS can be coded manually from scratch (using a combination of JS and CSS) or you can use a third-party JS framework.</li>
 	<li><em>For visually complex animations that are short, straight-forward, linear, and non-interactive,</em> consider using your favorite GUI (e.g. After Effects) to create an animated gif.</li>
 	<li><em>For longer form, dramatic narrative animations with complex visual effects,</em> consider there's always Video (HTML5 video).</li>
</ul>
[/et_pb_text][/et_pb_column][/et_pb_row][/et_pb_section][et_pb_section bb_built="1" fullwidth="off" specialty="off" prev_background_color="#000000" next_background_color="#000000"][et_pb_row][et_pb_column type="1_3"][et_pb_text admin_label="Section Heading and Sub-Heading" _builder_version="3.0.101" background_layout="light" module_class="text-single-column-narrow"]
<h2>CSS3 Animation</h2>
<em>Native Support in Most Browsers</em>

[/et_pb_text][et_pb_text admin_label="Section Content" _builder_version="3.0.101" background_layout="light" module_class="text-single-column-narrow"]
<ul>
 	<li>Native CSS properties used to animate elements (two approaches):
<ul>
 	<li><a href="https://www.w3schools.com/cssref/css3_pr_transition.asp">CSS transition</a></li>
 	<li><a href="https://www.w3schools.com/cssref/css3_pr_animation.asp">CSS animation</a> (via <a href="https://www.w3schools.com/cssref/css3_pr_animation-keyframes.asp">@keyframes</a>)</li>
</ul>
</li>
 	<li>Native CSS properties used to change elements (core):
<ul>
 	<li><a href="https://www.w3schools.com/cssref/css3_pr_transform.asp">CSS transform</a>
<ul>
 	<li>translate(<i>x,y</i>)</li>
 	<li>scale(<i>x,y</i>)</li>
 	<li>rotate(<i>angle</i>)</li>
</ul>
</li>
 	<li><a href="https://www.w3schools.com/cssref/css3_pr_opacity.asp">CSS opacity()</a></li>
</ul>
</li>
 	<li>3rd Party CSS Libraries (e.g. <a href="https://daneden.github.io/animate.css/">Animate.css</a>)</li>
</ul>
[/et_pb_text][/et_pb_column][et_pb_column type="1_3"][et_pb_text admin_label="Section Heading and Sub-Heading" _builder_version="3.0.101" background_layout="light" module_class="text-single-column-narrow"]
<h2>JS Animation</h2>
<em>Javascript animation via DOM manipulation</em>

[/et_pb_text][et_pb_text admin_label="Section Content" _builder_version="3.0.101" background_layout="light" module_class="text-single-column-narrow"]
<ul>
 	<li>Vanilla JS
<ul>
 	<li><a href="https://www.w3schools.com/js/js_htmldom_animate.asp">W3Schools Example</a> (uses both JS and CSS)</li>
</ul>
</li>
 	<li>JQuery
<ul>
 	<li><a href="https://www.w3schools.com/jquery/jquery_animate.asp">W3Schools JQuery animation page</a> + <a href="https://www.w3schools.com/jquery/tryit.asp?filename=tryjquery_animation1_multicss">example</a></li>
</ul>
</li>
 	<li>3rd Party JS Libraries
<ul>
 	<li><a href="https://greensock.com/gsap">GreenSock (GSAP)</a></li>
 	<li><a href="http://animejs.com/">Anime.js</a></li>
 	<li><a href="http://velocityjs.org/">Velocity.js</a></li>
 	<li><a href="http://mojs.io/">Mo.js</a></li>
</ul>
</li>
</ul>
[/et_pb_text][/et_pb_column][et_pb_column type="1_3"][et_pb_text admin_label="Section Heading and Sub-Heading" _builder_version="3.0.101" background_layout="light" module_class="text-single-column-narrow"]
<h2>Others</h2>
<i>Animated Gifs, HTML5 Video, HTML5 Canvas, and more...</i>

[/et_pb_text][et_pb_text admin_label="Section Content" _builder_version="3.0.101" background_layout="light" module_class="text-single-column-narrow"]
<ul>
 	<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Web_Animations_API">Web Animations API (WAAPI)</a></li>
 	<li>Classic, well-supported GUI-based approaches:
<ul>
 	<li>Animated Gif's</li>
 	<li>HTML5 Video</li>
</ul>
</li>
 	<li>Web-specific GUI-based approach:
<ul>
 	<li><a href="https://www.adobe.com/products/animate.html">Adobe Animate</a> (e.g. to export HTML5 Canvas)</li>
</ul>
</li>
 	<li>SVG Animation</li>
 	<li>Scroll-triggered Animations</li>
 	<li>Page Transitions (e.g. <a href="http://barbajs.org/">Barba.js</a>)</li>
 	<li>Mobile-UI Frameworks (e.g. JQuery Mobile, <a href="https://framework7.io/">Framework 7,</a> <a href="https://ionicframework.com/">Ionic</a>, etc)</li>
</ul>
[/et_pb_text][/et_pb_column][/et_pb_row][/et_pb_section][et_pb_section bb_built="1" fullwidth="off" specialty="off" _builder_version="3.0.89" next_background_color="#333333" prev_background_color="#000000"][et_pb_row][et_pb_column type="4_4"][et_pb_text admin_label="Text - Single Column Narrow" _builder_version="3.0.101" background_layout="light" module_class="text-single-column-narrow" saved_tabs="all"]
<h2>A Brief History</h2>
When trying to determine which web animation techniques are best amongst the many options available today, be sure to keep in mind the many different contexts and types of scenarios that exists for different web animations on the web today. For example, there are a growing number of UI animations, including micro-animations, that are becoming effective means of creating a better, more meaningful interfaces with a direct and positive impact on improving user experiences. Examples include animation navigation menus and menu icons, animated accordions, animated overlays, and animated form elements. Taken one notch further, UI animation includes animated page (or "state") transitions, such as the slide-left and slide-right transitions commonly found in many native mobile apps.

When it comes to content, many interfaces use animation to reveal, or present content using techniques such as fading, scaling, and sliding in content on page load and triggered animation based on user interactions and navigation, such as via page scrolling. Taken a step further, UI content in not only revealed, but also animated to illustrate custom content features, using elements such as custom animated illustrations and icons, and visual storytelling via vertical and horizontal scrolling. Taken further, there are full-blown time-based, linear time-based animation, such as animated advertisements and narrative motion graphics. Going even further, there are browser-based games that combine animation and interactivity in non-linear formats, along with code-generated artwork, three-dimensional worlds, and full-blown physics engines with particle systems and complex visual effects one might see in a medium like TV or film.

Check out this article entitled <a href="https://uxplanet.org/popular-web-animation-techniques-a6a467309028">Popular Web Animation Techniques</a> by Nick Babich with visual examples of some of the contexts mentioned above.

Given the wide range of contexts for several different applied use cases of animation on the web, one approach is to do the same with the many different technologies and tools available today, and then match them with an appropriate context.

[/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row][et_pb_column type="1_4"][/et_pb_column][et_pb_column type="1_2"][et_pb_testimonial _builder_version="3.0.101" author="Mark Geyer" url="http://markgeyer.com/pres/the-art-of-ui-animations/#/5/5" url_new_window="off" quote_icon="on" use_background_color="on" quote_icon_background_color="#f5f5f5" background_layout="light"]

You'll want to stick to transitioning transform and opacity as much as possible.

[/et_pb_testimonial][/et_pb_column][et_pb_column type="1_4"][/et_pb_column][/et_pb_row][et_pb_row _builder_version="3.0.89"][et_pb_column type="4_4"][et_pb_text admin_label="Text - Single Column Narrow" _builder_version="3.0.101" background_layout="light" module_class="text-single-column-narrow" saved_tabs="all"]
<h2>CSS3 animation techniques</h2>
For simple UI animations on the web, such as animated menus and UI components, CSS3 animation is probably going to offer the best support and performance across browsers. But wait, there are multiple ways to animate things using CSS3 Animation, so where to begin? CSS animation with keyframes? CSS transitions? Start by asking about the context: is this a UI animation with two states (A &gt; B) and trigger via a user interaction (user hovers or clicks), then CSS transitions are probably going to the simplest and easiest.
<h3><a href="https://www.w3schools.com/cssref/css3_pr_transition.asp">CSS Transitions</a></h3>
<pre><code>
transition: all 1s ease;
</code></pre>
<h3><a href="https://www.w3schools.com/cssref/css3_pr_animation.asp">CSS Animation</a> <a href="https://www.w3schools.com/cssref/css3_pr_animation-keyframes.asp">@Keyframes</a></h3>
If something needs to animate without any user interaction (or without using javascript), or if the animation contains more than just two states (e.g. A &gt; B &gt; C &gt; D), then CSS animation and @keyframes should work well.
<pre><code>
@keyframes fade-in {
from { transform: opacity: 0; }
to { transform: opacity: 1; }
}
.fade-in {
opacity: 0;
animation: fade-in 1s ease-in-out 1s forwards;
}
</code></pre>
<h3><a href="https://www.w3schools.com/cssref/css3_pr_transform.asp">CSS Transforms</a></h3>
Regardless of whether you choose CSS Transition or CSS animation, both can utilize the power of CSS Transforms. CSS transforms can translate, rotate, and scale HTML elements. Together with opacity, one can do amazing animations with these simple tools.

<strong>Four Core CSS Properties to use for CSS Animation:</strong>
<ol>
 	<li>position/translation: translate(x,y)</li>
 	<li>scale: scale(x,y)</li>
 	<li>rotation: rotate(angle)</li>
 	<li>opacity: opacity(value);</li>
</ol>
<h3>3rd Party CSS Libraries</h3>
If the effect that you or your client needs is not easily able to achieved via native CSS, there are several third-party CSS animation libraries to check out. They are also fun to peruse for visual inspiration.
<ul>
 	<li><a href="http://www.justinaguilar.com/animations/index.html">Animations.css</a></li>
 	<li><a href="https://daneden.github.io/animate.css/">Animate.css</a></li>
 	<li><a href="http://kristofferandreasen.github.io/wickedCSS/">Wicked.css</a></li>
 	<li><a href="https://minimamente.com/example/magic_animations/">Magic CSS</a></li>
</ul>
<h2></h2>
<h2>Javascript (JS) Animations</h2>
One level up from Native CSS animations are Javascript animations. There are multiple approaches and ways to use Javascript to create web animations, from writing native/vanilla JS, to JQuery, to 3rd party libraries.
<h3>Native JS</h3>
Vanilla JS, alone or in combination with CSS, is an effective and well-supported way to create browser-based web animations. Essentially Javascript is used to change the properties of elements on the page via DOM manipulation. This can be done directly (e.g. changing an elements properties using javascript) or indirectly (e.g. adding/removing a class on an element that is then changed via CSS3 animation). For a working example, check out this <a href="https://www.w3schools.com/js/js_htmldom_animate.asp">W3Schools example that uses both JS and CSS.</a>
<h3>JQuery</h3>
JQuery's .animate is a quick and easy approach. Check out <a href="https://www.w3schools.com/jquery/jquery_animate.asp">W3Schools JQuery animation page</a> to learn more and to see some demo examples, <a href="https://www.w3schools.com/jquery/tryit.asp?filename=tryjquery_animation1_multicss">like this one.</a>
<h3>3rd Party JS Libraries</h3>
If your needs are not easily able to achieved via native JS or Jquery, there are several third-party JS animation libraries to check out.
<ul>
 	<li><a href="https://greensock.com/gsap">GreenSock (GSAP)</a></li>
 	<li><a href="http://animejs.com/">Anime.js</a></li>
 	<li><a href="http://velocityjs.org/">Velocity.js</a></li>
 	<li><a href="http://mojs.io/">Mo.js</a></li>
</ul>
<h3></h3>
<h3>Web Animations API (WAAPI)</h3>
The <a href="https://developer.mozilla.org/en-US/docs/Web/API/Web_Animations_API">Web Animations API</a> is an important thing to monitor in the years to come. Currently, <a href="https://caniuse.com/#feat=web-animation">browser support for WAAPI</a> is relatively poor (compared to the other options presented on this page, although there is supposedly an OK polyfill), but this might be the future of animation on the web. Keep an eye on it.

[/et_pb_text][et_pb_text admin_label="Text - Single Column Narrow" _builder_version="3.0.101" background_layout="light" module_class="text-single-column-narrow" saved_tabs="all"]
<h2>Other Approaches, Techniques, and Technologies to Consider:</h2>
<h5>Page Transitions:</h5>
<ul>
 	<li><a href="http://barbajs.org/">Barba.js</a></li>
 	<li>Helpful links/examples/articles:
<ul>
 	<li><a href="http://freefrontend.com/css-page-transitions/">http://freefrontend.com/css-page-transitions/</a></li>
 	<li><a href="https://css-tricks.com/add-page-transitions-css-smoothstate-js/">https://css-tricks.com/add-page-transitions-css-smoothstate-js/</a></li>
 	<li><a href="https://tympanus.net/Development/PageTransitions/">https://tympanus.net/Development/PageTransitions/</a></li>
 	<li><a href="https://www.smashingmagazine.com/2016/07/improving-user-flow-through-page-transitions/">https://www.smashingmagazine.com/2016/07/improving-user-flow-through-page-transitions/</a></li>
</ul>
</li>
</ul>
<h5>Sprite Animations</h5>
<ul>
 	<li>[ Links coming soon... sorry! ]</li>
</ul>
<h5>SVG Animation</h5>
SVG Animation is an effective approach for vector-based imagery, such as icons and illustrations. Similar to other HTML elements, SVG's can be animated using CSS, JS, and/or a combination of these technologies.
<ul>
 	<li>[ Links coming soon... sorry! ]</li>
</ul>
<h5>Scroll-triggered animation</h5>
Animations that are triggered as the user scrolls on a page often times use Javascript for triggering (to detect when an element is within the viewport of a screen while the user is scrolling) and CSS for the animation (e.g. by adding/removing a class on an element).
<ul>
 	<li>Article with demo: <a href="https://ihatetomatoes.net/one-page-scroll-with-animations/">https://ihatetomatoes.net/one-page-scroll-with-animations/</a></li>
 	<li>Sample Breakdown article: <a href="https://ihatetomatoes.net/apple-iphone-5c-page-deconstructed/">https://ihatetomatoes.net/apple-iphone-5c-page-deconstructed/</a></li>
 	<li><a href="https://scrollrevealjs.org/">ScrollReveal.js</a></li>
</ul>
[/et_pb_text][et_pb_text admin_label="Text - Single Column Narrow" _builder_version="3.0.101" background_layout="light" module_class="text-single-column-narrow" saved_tabs="all"]
<h2>The Principles of Animation</h2>
No matter what, don't forget the basics of strong animation and motion graphic design. To remind yourself of the core principles of animation, watch this <a href="https://vimeo.com/93206523">Illusion of Life animation</a>.

<iframe src="https://player.vimeo.com/video/93206523" width="640" height="254" frameborder="0" allowfullscreen="allowfullscreen"></iframe>

<a href="https://vimeo.com/93206523">The illusion of life</a> from <a href="https://vimeo.com/centodesign">cento lodigiani</a> on <a href="https://vimeo.com">Vimeo</a>.

&nbsp;

[/et_pb_text][/et_pb_column][/et_pb_row][/et_pb_section][et_pb_section bb_built="1" fullwidth="off" specialty="off" _builder_version="3.0.89" background_color="#333333" prev_background_color="#ffffff" next_background_color="#ffffff"][et_pb_row _builder_version="3.0.89"][et_pb_column type="1_4"][/et_pb_column][et_pb_column type="1_2"][et_pb_blurb admin_label="Quick Hands-on Exercise Blurb" _builder_version="3.0.101" title="Quick Hands-on Exercise" url_new_window="off" use_icon="on" font_icon="%%92%%" use_circle="off" use_circle_border="off" icon_placement="top" use_icon_font_size="off" background_layout="dark" icon_color="#ffffff" text_orientation="center" header_level="h2"]

Try to solve the challenge below by doing the following: in the code examples below, click on the "edit in codepen" button in the upper right, then delete the css and try to recreate the original from scratch.

[/et_pb_blurb][/et_pb_column][et_pb_column type="1_4"][/et_pb_column][/et_pb_row][et_pb_row][et_pb_column type="4_4"][et_pb_text admin_label="Embedded CodePen" _builder_version="3.0.101" background_layout="dark" text_orientation="center" module_alignment="center"]
<h4>CSS Animation Exercise #1: Simple Fade-in Using @keyframes</h4>
[codepen_embed height="500" theme_id="0" slug_hash="zRzQQW" default_tab="css,result" user="kccnma"]See the Pen &lt;a href='https://codepen.io/kccnma/pen/zRzQQW/'&gt;CSS Animation Test: Simple Fade-in Using @keyframes&lt;/a&gt; by kccnma (&lt;a href='https://codepen.io/kccnma'&gt;@kccnma&lt;/a&gt;) on &lt;a href='https://codepen.io'&gt;CodePen&lt;/a&gt;.[/codepen_embed]

Instructions: remove all fade-in css and try to re-do it from scratch.

[/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row][et_pb_column type="4_4"][et_pb_text admin_label="Embedded CodePen" _builder_version="3.0.101" background_layout="dark" text_orientation="center" module_alignment="center"]
<h4>CSS Animation Exercise #2: Simple Scale-in Using @keyframes</h4>
[codepen_embed height="500" theme_id="0" slug_hash="ddRBpB" default_tab="css,result" user="kccnma"]See the Pen &lt;a href='https://codepen.io/kccnma/pen/ddRBpB/'&gt;CSS Animation Test: Simple Scale-in Using @keyframes&lt;/a&gt; by kccnma (&lt;a href='https://codepen.io/kccnma'&gt;@kccnma&lt;/a&gt;) on &lt;a href='https://codepen.io'&gt;CodePen&lt;/a&gt;.[/codepen_embed]

Instructions: remove all scale-in css and try to re-do it from scratch.

[/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row][et_pb_column type="4_4"][et_pb_text admin_label="Embedded CodePen" _builder_version="3.0.101" background_layout="dark" text_orientation="center" module_alignment="center"]
<h4>CSS Animation Exercise #2: Simple Move-in (and Fade-in) Using @keyframes</h4>
[codepen_embed height="500" theme_id="0" slug_hash="KQqjZZ" default_tab="css,result" user="kccnma"]See the Pen &lt;a href='https://codepen.io/kccnma/pen/KQqjZZ/'&gt;CSS Animation Test: Simple Move-in Using @keyframes&lt;/a&gt; by kccnma (&lt;a href='https://codepen.io/kccnma'&gt;@kccnma&lt;/a&gt;) on &lt;a href='https://codepen.io'&gt;CodePen&lt;/a&gt;.[/codepen_embed]

Instructions: remove all move-in css and try to re-do it from scratch.

[/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row][et_pb_column type="4_4"][et_pb_text admin_label="Embedded CodePen" _builder_version="3.0.101" background_layout="dark" text_orientation="center" module_alignment="center"]
<h4>CSS Animation Exercise #4: CSS3 Animation Hero Section Examples</h4>
[codepen_embed height="600" theme_id="0" slug_hash="wmgRRP" default_tab="css,result" user="kccnma"]See the Pen &lt;a href='https://codepen.io/kccnma/pen/wmgRRP/'&gt;CSS3 Animation Header and Hero Section Example&lt;/a&gt; by kccnma (&lt;a href='https://codepen.io/kccnma'&gt;@kccnma&lt;/a&gt;) on &lt;a href='https://codepen.io'&gt;CodePen&lt;/a&gt;.[/codepen_embed]

Instructions: remove all css and try to re-do it from scratch.

[/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row][et_pb_column type="4_4"][et_pb_text admin_label="Embedded CodePen" _builder_version="3.0.101" background_layout="dark" text_orientation="center" module_alignment="center"]
<h4>CSS Animation Exercise #4: CSS3 Animation Hero Section Examples</h4>
[codepen_embed height="600" theme_id="0" slug_hash="oqBmQG" default_tab="css,result" user="kccnma"]See the Pen &lt;a href='https://codepen.io/kccnma/pen/oqBmQG/'&gt;CSS3 Animation Header and Hero Section Example&lt;/a&gt; by kccnma (&lt;a href='https://codepen.io/kccnma'&gt;@kccnma&lt;/a&gt;) on &lt;a href='https://codepen.io'&gt;CodePen&lt;/a&gt;.[/codepen_embed]

Instructions: remove all css and try to re-do it from scratch.

[/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row _builder_version="3.0.89"][et_pb_column type="1_4"][/et_pb_column][et_pb_column type="1_2"][et_pb_blurb admin_label="Quick Hands-on Exercise Blurb" _builder_version="3.0.101" title="Good Job!" url_new_window="off" use_icon="on" font_icon="%%277%%" use_circle="off" use_circle_border="off" icon_placement="top" use_icon_font_size="on" background_layout="dark" icon_color="#ffffff" text_orientation="center" icon_font_size="32px"]

If you completed these exercises, nice work! Keep reading to learn more...

[/et_pb_blurb][/et_pb_column][et_pb_column type="1_4"][/et_pb_column][/et_pb_row][/et_pb_section][et_pb_section bb_built="1" fullwidth="off" specialty="off" prev_background_color="#333333" next_background_color="#000000"][et_pb_row][et_pb_column type="4_4"][et_pb_text admin_label="Conclusion" _builder_version="3.0.101" background_layout="light" module_class="text-single-column-narrow"]
<h2>Conclusion</h2>
There are multiple different ways to animate on the web. For UI based animation, the simplest and easiest way is to use CSS3 animation. When relatively simple user interactivity is required, you can add in a light amount of Javascript for DOM manipulation. For more complex UI web animations, such as scroll-triggered animations and animated page transitions, more advanced Javascript is required. These can be coded manually, from scratch (using a combination of JS and CSS), or you can use a third-party JS framework. For visually complex animations that are short, straight-forward, linear, and non-interactive, consider using an animated gif.  For longer form, dramatic narrative animations with complex visual effects, there's always HTML5 Video.

When trying to determine which web animation techniques are best amongst the many options available today, be sure to keep in mind the overall size of the files and all dependencies required and the performance implications on the browser during page load (e.g. a large SVG that is greater than 1MB might be better displayed as either layered pngs or even an animated gif). Often times the best practice is to do a series of tests experimenting with several different techniques, then critically weigh the pro's and cons for each before making a decision. Regardless of the technologies used, be sure to use UI animation with a clear and thoughtful purpose that will result in a meaningful interface with a positive impact on improving the user experience.

&nbsp;

[/et_pb_text][/et_pb_column][/et_pb_row][/et_pb_section][et_pb_section bb_built="1" fullwidth="off" specialty="off" prev_background_color="#000000"][et_pb_row][et_pb_column type="4_4"][et_pb_text admin_label="Related Resources" _builder_version="3.0.101" background_layout="light" module_class="text-single-column-narrow"]
<h3>Related Resources and Reading</h3>
<ul>
 	<li>Rachel Nabor's <a href="https://abookapart.com/products/animation-at-work">Animation at Work Book</a></li>
 	<li>Rachel Nabor's <a href="http://alistapart.com/article/web-animation-at-work">2014 ALA Web Animation at Work Article</a></li>
 	<li><a href="https://robots.thoughtbot.com/css-animation-for-beginners">CSS Animation for Beginners</a> by Rachel Cope</li>
 	<li>Mark Geyer's <a href="http://markgeyer.com/pres/the-art-of-ui-animations/#/">Web Animation Presentation</a></li>
 	<li><a href="https://matthewlein.com/tools/ceaser">Caesar</a>, a CSS Easing Tool</li>
 	<li><a href="https://webdesign.tutsplus.com/tutorials/a-beginners-introduction-to-css-animation--cms-21068">Beginners Guide to CSS Animation</a></li>
 	<li><a href="http://www.valhead.com/">Val Head</a>'s Many Resources, including her book <a href="https://rosenfeldmedia.com/books/designing-interface-animation/">Designing Interface Animation</a></li>
</ul>
<h3>Inspiration:</h3>
<ul>
 	<li><a href="https://delaneau.com/">https://delaneau.com/</a></li>
 	<li><a href="https://www.psd2html.com/10-years-in-review/">https://www.psd2html.com/10-years-in-review/</a></li>
 	<li><a href="https://www.apple.com/mac-pro/">https://www.apple.com/mac-pro/</a> (old school, no longer live?)</li>
 	<li><a href="https://ihatetomatoes.net/apple-mac-pro-page-deconstructed/">https://ihatetomatoes.net/apple-mac-pro-page-deconstructed/</a></li>
 	<li><a href="http://madebytheory.com/">http://madebytheory.com/</a> (simple and subtle)</li>
 	<li><a href="https://humaan.com/">https://humaan.com/</a></li>
</ul>
&nbsp;
<h3>Examples:</h3>
<ul>
 	<li><a href="https://envato.com/blog/subtly-animated-forms/">Animated Forms</a></li>
 	<li><a href="https://speckyboy.com/page-transition-effects/">10 Exciting Page Transition Effects</a> (via Speckyboy)</li>
</ul>
<h3>Systems:</h3>
<ul>
 	<li><a href="https://material.io/guidelines/motion/material-motion.html">Google's Material Design</a></li>
 	<li><a href="https://www.lightningdesignsystem.com/guidelines/animation/styleguidelines/#content">Salesforce's Lighting System</a>
<ul>
 	<li><a href="https://www.salesforce.com/video/194256/">Choreographed Animations Video</a></li>
</ul>
</li>
</ul>
&nbsp;

[/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row _builder_version="3.0.101"][et_pb_column type="4_4"][et_pb_text admin_label="Go Further" _builder_version="3.0.101" background_layout="light" module_class="text-single-column-narrow"]
<h3>Go Further</h3>
<ul>
 	<li>Try animation a page's header and hero content like this <a href="https://codepen.io/kccnma/pen/oqBmQG?editors=1100">Codepen Example</a></li>
 	<li>Try revealing content as a user scrolls down the page like this <a href="https://codepen.io/kccnma/pen/MQeXPY">Codepen Example</a></li>
</ul>
[/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row][et_pb_column type="4_4"][et_pb_toggle admin_label="Author Notes" _builder_version="3.0.101" title="Author Notes" open="off" module_class="text-single-column-narrow"]
<h6>This was written specifically to help aspiring web designers as they aim to:</h6>
<ul>
 	<li>Learn the basic concepts and principles of web animation</li>
 	<li>Learn how the basic principles of motion graphic design can be applied in the context of user interface design</li>
 	<li>Use animation and motion design technologies and techniques to enhance the user experience.</li>
</ul>
[/et_pb_toggle][/et_pb_column][/et_pb_row][/et_pb_section]