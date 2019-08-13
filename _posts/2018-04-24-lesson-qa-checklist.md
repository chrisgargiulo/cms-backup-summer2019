---
ID: 1771
post_title: Quality Assurance Checklist
author: CMS
post_excerpt: ""
layout: post
permalink: >
  https://creativemedia.space/lesson-qa-checklist/
published: true
post_date: 2018-04-24 14:18:03
---
<!-- wp:heading {"level":3} -->
<h3>Pre-launch QA Diligence</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Prior to the launch of web sites both big and small, there are several techniques and best practices to help ensure the delivery of a quality product that is performant and bug free. Often times addressed toward the end of a project, one of the most commonly used terms to describe this step of the process is <em>quality assurance</em>, or <em>QA</em>.</p>
<!-- /wp:paragraph -->

<!-- wp:more -->
<!--more-->
<!-- /wp:more -->

<!-- wp:quote -->
<blockquote class="wp-block-quote"><p><strong>Quality assurance (QA)</strong> is a way of preventing mistakes and defects in manufactured products and avoiding problems when delivering solutions or services to customers<br> – <a href="https://en.wikipedia.org/wiki/Quality_assurance">Wikipedia</a></p></blockquote>
<!-- /wp:quote -->

<!-- wp:heading -->
<h2>Bug Tracking</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><em>Validate, Fix Errors, Manage Enhancements</em></p>
<!-- /wp:paragraph -->

<!-- wp:list -->
<ul><li>Track and Prioritize your Bugs and Tasks
<ul><li>Online tools: Google Spreadsheets (<a href="https://docs.google.com/spreadsheets/d/1mHutADPn3odgTXmKIdpQCUIQdEGx_lnlLXhWauReM8k/edit?usp=sharing">Example QA Bug Tracking Sheet</a>), Trello Boards (<a href="https://trello.com/b/ppAc7F3k/project-bug-tracking-list">Example Trello Bug Tracking Board</a>), <a href="https://guides.github.com/features/issues/">Github Issues</a>, etc.</li></ul>
</li><li>Validate your code
<ul><li><a href="https://validator.w3.org/">Validate HTML</a></li><li><a href="http://jigsaw.w3.org/css-validator/">Validate CSS</a></li><li><a href="http://wave.webaim.org/">Validate Accessibility</a> (Section 508 compliance)
<ul><li>Provide "equivalent" experience to all users. For example, make sure all img alt tags are appropriate.</li><li>Check out online resources, such as:&nbsp;The <a href="https://www.w3.org/WAI/">W3C Web Accessibility Initiative (WAI)</a> and <a href="https://www.w3.org/WAI/yourWAI">their list of resources</a>, the&nbsp;<a href="https://a11yproject.com/">A11Y Project</a>, <a href="https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA">ARIA</a>, etc.</li></ul>
</li></ul>
</li><li>Test in multiple Platforms, Browsers, Screen Sizes, and Devices
<ul><li>Example of online Tools: <a href="https://www.browserling.com/">Browserling</a>, <a href="https://netrenderer.com/index.php">Netrenderer</a>, <a href="https://saucelabs.com/">Sauce Labs</a>, <a href="https://www.browserstack.com/pricing?tab=browser-plans-tab">Browserstack</a>, <a href="http://browsershots.org/">Browsershots</a>, <a href="https://developers.google.com/web/tools/chrome-devtools/device-mode/">Chrome's Device Mode</a></li></ul>
</li></ul>
<!-- /wp:list -->

<!-- wp:heading -->
<h2>Performance Enhancements</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><em>Techniques to improve the speed of your site</em></p>
<!-- /wp:paragraph -->

<!-- wp:list -->
<ul><li>Test your site at <a href="https://web.dev/">web.dev&nbsp;</a>and <a href="https://developers.google.com/speed/pagespeed/insights/">Google Page Speed Insights</a></li><li>Conduct a site audit for K size of all assets</li><li>Optimize all media (e.g. images, videos, etc). Example: manually adjust via Photoshop's Save for the web (legacy). Recommended Image Formats:
<ul><li>jpg (for images/raster photos with lots of color)</li><li>gif (for images/illustration with under 256 colors)</li><li>png-24 (for images that require alpha transparency</li></ul>
</li></ul>
<!-- /wp:list -->

<!-- wp:list -->
<ul><li>Minify all local dependencies (html, css, and js)</li><li>Considerations:
<ul><li>Consider using a CDN</li><li>Consider using a <a href="https://www.smashingmagazine.com/2015/08/understanding-critical-css/">critical css</a> file</li><li>Consider file compression (e.g. gzip)</li></ul>
</li></ul>
<!-- /wp:list -->

<!-- wp:heading -->
<h2>Due Diligence</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><em>Style guides, code clean-up, and more...</em></p>
<!-- /wp:paragraph -->

<!-- wp:list -->
<ul><li>Refactor all code by removing any redundant or unnecessary code. <ul><li>Remove unused markup (html)</li><li>Remove unused styling (css)</li><li>Concatenate your Javascript into one js file </li></ul></li><li>Consider creating in-house style guidelines &amp; documentation (for internal developer use and/or client use).</li></ul>
<!-- /wp:list -->

<!-- wp:heading -->
<h2>Quick Checklist</h2>
<!-- /wp:heading -->

<!-- wp:list {"ordered":true} -->
<ol><li>Is your HTML &amp; CSS validating with no errors?</li><li>Is your site Section 508 Compliant?</li><li>Have you tested on Multiple Platforms, Browsers, Devices, and Screen Sizes?
<ul><li>Mac and PC</li><li>Chrome, Firefox, Safari, IE, Edge</li><li>Large Monitor, Laptop Display, Tablet, Mobile (including portrait &amp; landscape views)</li><li>iOS and Android</li></ul>
</li><li>Have you done a site audit and optimized all assets and media (images, videos, etc.)?</li></ol>
<!-- /wp:list -->