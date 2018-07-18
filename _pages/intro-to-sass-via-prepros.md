---
ID: 338
post_title: Intro to SASS via Prepros
author: CMS
post_excerpt: ""
layout: page
permalink: >
  https://www.creativemedia.space/lessons/intro-to-sass-via-prepros/
published: true
post_date: 2017-08-31 06:50:49
---
[et_pb_section bb_built="1" fullwidth="on" specialty="off" next_background_color="#000000"][et_pb_fullwidth_image _builder_version="3.0.85" src="https://www.creativemedia.space/wp-content/uploads/2017/08/sass-prepros-4x1.gif" show_in_lightbox="off" url_new_window="off" use_overlay="off" /][/et_pb_section][et_pb_section bb_built="1" prev_background_color="#000000"][et_pb_row][et_pb_column type="4_4"][et_pb_text admin_label="Title - Single Column Narrow" _builder_version="3.0.106" background_layout="light" module_class="text-single-column-narrow"]
<h1>Introduction to SASS via Prepros</h1>
<em>Organizing Styles: Using SASS Partials for a Modular CSS Setup</em>

[/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row][et_pb_column type="4_4"][et_pb_text admin_label="Text - Single Column Narrow" _builder_version="3.0.106" background_layout="light" module_class="text-single-column-narrow"]
<h3>Summary</h3>
How you choose to organize your styles can affect your efficiency as a front-end developer (how long it takes you to write code? how much code do you re-use from project to project? ), your ability to manage complex projects and work with others (how readable is your code? how easily can others understand it?), and how fast your site loads (how how much of that code is actually needed? do you always make time to refactor and optimize your code?).

This may not be a big concern for small static brochure sites, but as you work on larger, more complex projects with multiple designers/developers, style organization becomes essential. One solution is to separate your styles into smaller parts (partials) and then use a preprocessor (SASS) to compile the styles into one style.css.

In this lesson, we will work backwards: using a stylesheet for a small brochure site, we will convert a single-file CSS system into an organized multi-file SASS system. The end product, a “compiled” style.css file, should be no different than it was in the beginning. However, the new organizational system (scss folder with partials) and new workflow (using a local dev environment) will provide a faster, more efficient way to write code, a cleaner, more maintainable code base that is re-usable, and a more powerful, flexible way to export and deploy project styles.

&nbsp;
<h4>Outcomes:</h4>
<ul>
 	<li>Spin up a local web server from a dev environment (as opposed to using an IDE)</li>
 	<li>Auto-reload a browser whenever a file is saved without a manual refresh.</li>
 	<li>Auto-compile SASS (via a compiler/task manager that watches for changes)</li>
 	<li>Use SASS features to set up a modular style base for a small site (using SASS partials)</li>
</ul>
&nbsp;
<h4>Steps:</h4>
<ol>
 	<li><strong>Setup a local front-end web development environment to compile SASS.</strong> In this step, we  will use a Prepros, a GUI-based front-end compiler. In another lesson, we will use Gulp.</li>
 	<li><strong>Establish a custom organizational file system</strong> using SASS partials that embraces best practices and strategies from popular CSS methodologies (e.g. SMACSS).</li>
 	<li><strong>Convert the CSS to SASS</strong> by reverse engineering the original, singular CSS file and separating it into a modular system of multiple SASS partial files. The new SCSS files will embrace SASS features to improve the coding experience, such as variables and nesting.</li>
</ol>
&nbsp;

<hr />

&nbsp;
<h3>Step One</h3>
<img class="alignnone size-full wp-image-348" src="https://www.creativemedia.space/wp-content/uploads/2017/08/sitebase-sassy-step1.gif" alt="" width="1000" height="500" />
<h4>Download Starter Files</h4>
<ol>
 	<li>You can start with your own static base (e.g. in a previous lesson, you might have already created a static "My Base 1.0" based on <a href="https://github.com/kccnma/sitebase1-static">Site Base 1.0</a>) that you already may have already created on your own. If not,  you can download the provided <a href="https://github.com/kccnma/sitebase/blob/master/docs/versions/sitebase1.zip?raw=true">sitebase1.zip</a> or <a href="https://github.com/kccnma/teachingmaterials/blob/master/sitebase-static-css.zip?raw=true">sitebase-static-css.zip </a>and expand it in a local folder on your computer</li>
 	<li>Rename the project folder to sitebase-sassy</li>
 	<li>Rename style.css to style-orig.css</li>
 	<li>Create a new folder named “scss”
<ul>
 	<li>Inside of scss, create a new file names style.scss
<ul>
 	<li>Add a $text-color variable and set the body color to the variable</li>
</ul>
</li>
</ul>
</li>
</ol>
<img class="alignnone size-full wp-image-351" src="https://www.creativemedia.space/wp-content/uploads/2017/08/sitebase-sassy-step2.gif" alt="" width="1000" height="500" />
<h4>Setup a Local Environment using Prepros</h4>
<ol>
 	<li>Add sitebase-sassy project into prepros (drag &amp; drop folder)</li>
 	<li>Test sass compiling by editing style.scss
<ul>
 	<li>Ensure that a new style.css file is created and that the text turns red</li>
</ul>
</li>
 	<li>Use prepress “preview” to fire up a local web server</li>
</ol>
&nbsp;

<hr />

&nbsp;
<h3>Step Two</h3>
<h4>Create SASS Partials</h4>
<ol>
 	<li>Inside of your scss folder, create a new folder named “partials”</li>
 	<li>In your editor, open up style-orig.css for reference (e.g. on the right)</li>
 	<li>Open up style.scss (e.g. on the left)</li>
 	<li>We are going to take css from the right and copy-paste it into new .scss files that we will create from scratch.</li>
</ol>
<h4>Link SASS Partials via @import</h4>
<ul>
 	<li>Change the root stylesheet (style.scss) to import base (_base.scss)
<ul>
 	<li>@import "base";
<ul>
 	<li>Note: the @import statement does not include the underscore "_"</li>
</ul>
</li>
 	<li>optional: add site-specific comments after the base</li>
</ul>
</li>
 	<li>Create, then import all partials into "base"
<ul>
 	<li>Start by creating/adding variables (_variables.scss)</li>
 	<li>Then import it into base
<ul>
 	<li>@import "variables";</li>
</ul>
</li>
</ul>
</li>
 	<li>Order of files to create/add/import into base:
<ul>
 	<li>base.scss
<ol>
 	<li>@import "variables";</li>
 	<li>@import "partials/toc-base";</li>
 	<li>@import "partials/html5";</li>
 	<li>@import "partials/typography";</li>
 	<li>@import "partials/media";</li>
 	<li>@import "partials/components";</li>
 	<li>@import "partials/layout";</li>
 	<li>@import "partials/structure";</li>
 	<li>@import "partials/site-navigation";</li>
 	<li>@import "partials/site-navigation-togglenav";</li>
</ol>
</li>
</ul>
</li>
</ul>
In the end, your project folder look like this:
<pre><code>
sitebase-sassy/
└── css/
    ├── style.css (compiled/generated - OK to delete to test)
└── scss/
    ├── style.scss
    ├── _variables.scss
    ├── _base.scss
    ├── partials/
        ├── _toc-base.scss
        ├── _html5.scss
        ├── _typography.scss
        ├── _media.scss
        ├── _components.scss
        ├── _layout.scss
        ├── _structure.scss
        ├── _site-navigation.scss
        ├── _site-navigation-togglenav.scss
</code></pre>
&nbsp;

You can also reference the folder structure and list of partial SCSS files via the end/completed lesson files here:
<ul>
 	<li><a href="https://github.com/kccnma/teachingmaterials/tree/master/sitebase-sassed">https://github.com/kccnma/teachingmaterials/tree/master/sitebase-sassed</a></li>
</ul>
&nbsp;

<hr />

&nbsp;
<h3>Step Three</h3>
<h4>Copy &amp; Paste from CSS to SCSS</h4>
<ol>
 	<li>Working from the top to the bottom, copy and paste css from style.css into the appropriate scss partial files.</li>
 	<li>As you copy and paste, convert the CSS to SCSS to embrace the following SASS features:
<ul>
 	<li>Variables: create new variables for any duplicate values</li>
 	<li>Nesting: nest and indent selectors when appropriate</li>
</ul>
</li>
 	<li>Test as you code</li>
</ol>
<h4>Customize</h4>
When you are done, you are welcome to customize this base and make it your own. For example, if you saved your static version as "My Base 1.0" then consider naming this new base to "My Base 2.0" and uploading it to github for future reference. Here are two such repositories from John Doe:
<ul>
 	<li>John Doe's <a href="https://github.com/johndoenma/mybase1">My Base 1.0</a></li>
 	<li>John Doe's <a href="https://github.com/johndoenma/mybase2">My Base 2.0</a></li>
</ul>
&nbsp;

<hr />

&nbsp;
<h4>Related Reading</h4>
<ul>
 	<li><a href="http://thesassway.com/beginner/how-to-structure-a-sass-project">How to structure a Sass project</a></li>
 	<li><a href="https://smacss.com/">SMACSS: Scalable and Modular Architecture for CSS</a></li>
 	<li><a href="http://getbem.com/introduction/">BEM: Blocks, Elements and Modifiers</a></li>
</ul>
&nbsp;
<h4>Lesson Resources:</h4>
<ul>
 	<li>Throughout this lesson, you can reference the start/beginning and end/completed lesson files here:
<ul>
 	<li><a href="https://github.com/kccnma/teachingmaterials/tree/master/sitebase-static-css">https://github.com/kccnma/teachingmaterials/tree/master/sitebase-static-css</a></li>
 	<li><a href="https://github.com/kccnma/teachingmaterials/tree/master/sitebase-sassed">https://github.com/kccnma/teachingmaterials/tree/master/sitebase-sassed</a></li>
</ul>
</li>
 	<li>You can also download the following archives (.zip files) of the lesson files here:
<ul>
 	<li><a href="https://github.com/kccnma/teachingmaterials/blob/master/sitebase-static-css.zip?raw=true">sitebase-static-css.zip </a></li>
 	<li><a href="https://github.com/kccnma/teachingmaterials/blob/master/sitebase-sassed.zip?raw=true">sitebase-sassed.zip </a></li>
</ul>
</li>
</ul>
[/et_pb_text][/et_pb_column][/et_pb_row][/et_pb_section]