---
ID: 1771
post_title: Quality Assurance Checklist
author: Front-end Freddy
post_excerpt: ""
layout: post
permalink: >
  https://www.creativemedia.space/lesson-qa-checklist/
published: true
post_date: 2018-04-24 14:18:03
---
[et_pb_section bb_built="1" _builder_version="3.0.89" next_background_color="#000000"][et_pb_row _builder_version="3.0.47" background_size="initial" background_position="top_left" background_repeat="repeat"][et_pb_column type="4_4"][et_pb_image src="https://www.creativemedia.space/wp-content/uploads/2018/04/checklist-4x2.gif" _builder_version="3.0.106"]
[/et_pb_image][/et_pb_column][/et_pb_row][et_pb_row _builder_version="3.0.89"][et_pb_column type="4_4"][et_pb_text admin_label="Running Head" module_class="articlerunninghead text-single-column-narrow" _builder_version="3.0.89"]

Lesson

[/et_pb_text][et_pb_text admin_label="Title and Subtitle" module_class="lesson-summary text-single-column-narrow" _builder_version="3.0.106" module_alignment="center"]
<h1>Quality Assurance Checklist</h1>
<h2>Pre-launch QA Diligence</h2>
[/et_pb_text][et_pb_post_title title="off" date="off" categories="off" comments="off" featured_image="off" module_class="lesson-summary text-single-column-narrow" _builder_version="3.0.106"]
[/et_pb_post_title][et_pb_text admin_label="Summary Text - Single Column Narrow" module_class="text-single-column-narrow" _builder_version="3.0.106" saved_tabs="all"]

Prior to the launch of web sites both big and small, there are several techniques and best practices to help ensure the delivery of a quality product that is performant and bug free. Often times addressed toward the end of a project, one of the most commonly used terms to describe this step of the process is <em>quality assurance</em>, or <em>QA</em>.
<blockquote><strong>Quality assurance (QA)</strong> is a way of preventing mistakes and defects in manufactured products and avoiding problems when delivering solutions or services to customers
<cite> – <a href="https://en.wikipedia.org/wiki/Quality_assurance">Wikipedia</a></cite></blockquote>
[/et_pb_text][/et_pb_column][/et_pb_row][/et_pb_section][et_pb_section bb_built="1" _builder_version="3.0.47" prev_background_color="#000000" next_background_color="#000000"][et_pb_row _builder_version="3.0.47" background_size="initial" background_position="top_left" background_repeat="repeat"][et_pb_column type="1_3"][et_pb_text admin_label="Section Heading and Sub-Heading" module_class="text-single-column-narrow" _builder_version="3.0.106"]
<h2>Bug Tracking</h2>
<i>Validate, Fix Errors, Manage Enhancements</i>

[/et_pb_text][et_pb_text admin_label="Section Content" module_class="text-single-column-narrow" _builder_version="3.0.106"]
<ul>
 	<li>Track and Prioritize your Bugs and Tasks
<ul>
 	<li>Online tools: Google Spreadsheets (<a href="https://docs.google.com/spreadsheets/d/1mHutADPn3odgTXmKIdpQCUIQdEGx_lnlLXhWauReM8k/edit?usp=sharing">Example QA Bug Tracking Sheet</a>), Trello Boards (<a href="https://trello.com/b/ppAc7F3k/project-bug-tracking-list">Example Trello Bug Tracking Board</a>), <a href="https://guides.github.com/features/issues/">Github Issues</a>, etc.</li>
</ul>
</li>
 	<li>Validate your code
<ul>
 	<li><a href="https://validator.w3.org/">Validate HTML</a></li>
 	<li><a href="http://jigsaw.w3.org/css-validator/">Validate CSS</a></li>
 	<li><a href="http://wave.webaim.org/">Validate Accessibility</a> (Section 508 compliance)
<ul>
 	<li>Provide "equivalent" experience to all users. For example, make sure all img alt tags are appropriate.</li>
</ul>
</li>
</ul>
</li>
 	<li>Test in multiple Platforms, Browsers, Screen Sizes, and Devices
<ul>
 	<li>Online Tools: <a href="https://www.browserling.com/">Browserling</a>, <a href="https://netrenderer.com/index.php">Netrenderer</a>, <a href="https://saucelabs.com/">Sauce Labs</a>, <a href="https://www.browserstack.com/pricing?tab=browser-plans-tab">Browserstack</a>, <a href="http://browsershots.org/">Browsershots</a>, <a href="https://developers.google.com/web/tools/chrome-devtools/device-mode/">Chrome's Device Mode</a></li>
</ul>
</li>
</ul>
[/et_pb_text][/et_pb_column][et_pb_column type="1_3"][et_pb_text admin_label="Section Heading and Sub-Heading" module_class="text-single-column-narrow" _builder_version="3.0.106"]
<h2>Performance Enhancements</h2>
<em>Techniques to improve the speed of your site</em>

[/et_pb_text][et_pb_text admin_label="Section Content" module_class="text-single-column-narrow" _builder_version="3.0.106" background_layout="light"]
<ul>
 	<li>Conduct a site audit for K size of all assets
<ul>
 	<li>Optimize all media (e.g. images, videos, etc). Example: manually adjust via Photoshop's Save for the web (legacy). Recommended Image Formats:
<ul>
 	<li>jpg (for images/raster photos with lots of color)</li>
 	<li>gif (for images/illustration with under 256 colors)</li>
 	<li>png-24 (for images that require alpha transparency)</li>
</ul>
</li>
</ul>
</li>
 	<li>Minify all local dependencies (html, css, and js)</li>
 	<li>Considerations:
<ul>
 	<li>Consider using a CDN</li>
 	<li>Consider using a critical css file</li>
 	<li>Consider file compression (e.g. gzip)</li>
</ul>
</li>
</ul>
[/et_pb_text][/et_pb_column][et_pb_column type="1_3"][et_pb_text admin_label="Section Heading and Sub-Heading" module_class="text-single-column-narrow" _builder_version="3.0.106"]
<h2>Due Diligence</h2>
<i>Style guides, code clean-up, and more...</i>

[/et_pb_text][et_pb_text admin_label="Section Content" module_class="text-single-column-narrow" _builder_version="3.0.106"]
<ul>
 	<li>Refactor all code by removing any redundant or unnecessary code.
<ul>
 	<li>Remove unused markup (html)</li>
 	<li>Remove unused styling (css)</li>
 	<li>Concatenate your Javascript into one js file</li>
</ul>
</li>
 	<li>Consider creating in-house style guidelines &amp; documention (for internal developer use and/or client use).</li>
</ul>
[/et_pb_text][/et_pb_column][/et_pb_row][/et_pb_section][et_pb_section bb_built="1" _builder_version="3.0.47" prev_background_color="#000000"][et_pb_row _builder_version="3.0.47" background_size="initial" background_position="top_left" background_repeat="repeat"][et_pb_column type="4_4"][et_pb_text admin_label="Text - Single Column Narrow" module_class="text-single-column-narrow" _builder_version="3.0.106" saved_tabs="all"]
<h2>Quick Checklist</h2>
<ol>
 	<li>Is your HTML &amp; CSS validating with no errors?</li>
 	<li>Is your site Section 508 Compliant?</li>
 	<li>Have you tested on Multiple Platforms, Browsers, Devices, and Screen Sizes?
<ul>
 	<li>Mac and PC</li>
 	<li>Chrome, Firefox, Safari, IE, Edge</li>
 	<li>Large Monitor, Laptop Display, Tablet, Mobile (including portrait &amp; landscape views)</li>
 	<li>iOS and Android</li>
</ul>
</li>
 	<li>Have you done a site audit and optimized all assets and media (images, videos, etc.)?</li>
</ol>
[/et_pb_text][/et_pb_column][/et_pb_row][/et_pb_section]