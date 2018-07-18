---
ID: 1208
post_title: 'Assignment: Create a Course Web Site'
author: Marky Mark
post_excerpt: ""
layout: post
permalink: >
  https://www.creativemedia.space/assignment-create-a-course-web-site/
published: true
post_date: 2018-01-11 01:38:31
---
[et_pb_section bb_built="1" _builder_version="3.0.47"][et_pb_row _builder_version="3.0.47" background_size="initial" background_position="top_left" background_repeat="repeat"][et_pb_column type="4_4"][et_pb_image src="https://www.creativemedia.space/wp-content/uploads/2018/01/coursewebpage-4x2.gif" _builder_version="3.0.92" /][/et_pb_column][/et_pb_row][et_pb_row _builder_version="3.0.47" background_size="initial" background_position="top_left" background_repeat="repeat"][et_pb_column type="4_4"][et_pb_text admin_label="Running Head" module_class="articlerunninghead text-single-column-narrow" _builder_version="3.0.92"]

Assignment

[/et_pb_text][et_pb_text admin_label="Title and Subtitle" module_class="lesson-summary text-single-column-narrow" _builder_version="3.0.92" module_alignment="center"]

<h1>Create a Course Web Site</h1>
<h2>Setup a simple website from scratch</h2>

[/et_pb_text][et_pb_post_title title="off" date="off" comments="off" featured_image="off" module_class="lesson-summary text-single-column-narrow" _builder_version="3.0.92" /][et_pb_text admin_label="Introduction Summary and Outcomes" module_class="lesson-summary text-single-column-narrow" _builder_version="3.0.92"]

One of the best ways to learn about web design is to get your hands dirty and code a simple website from scratch. Having ones own domain and web site enables designers to learn through practice, by going through the full development process from beginning to end, from setting up a local development environment to deploying and maintaining a live site with continually changing content over time.

[/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row module_class="text-centered" _builder_version="3.0.89"][et_pb_column type="4_4"][et_pb_button admin_label="Demo Button" button_url="https://johndoenma.github.io/coursework/art128/index.html" button_text="See a Demo" button_alignment="center" _builder_version="3.0.92" custom_button="on" button_use_icon="off" /][et_pb_button admin_label="Watch a Video Lesson Button" button_url="#videolesson" button_text="Watch a Video Lesson" button_alignment="center" _builder_version="3.0.92" custom_button="on" button_use_icon="off" /][et_pb_button admin_label="Download Source Files Button" button_url="https://github.com/johndoenma/coursework/archive/master.zip" button_text="Download Source Files" button_alignment="center" _builder_version="3.0.92" custom_button="on" button_use_icon="off" /][et_pb_button admin_label="View on Github Button" button_url="https://github.com/johndoenma/coursework" button_text="View on Github" button_alignment="center" _builder_version="3.0.92" custom_button="on" button_use_icon="off" /][/et_pb_column][/et_pb_row][et_pb_row _builder_version="3.0.47" background_size="initial" background_position="top_left" background_repeat="repeat"][et_pb_column type="4_4"][et_pb_text admin_label="Introduction Summary and Outcomes" module_class="lesson-summary text-single-column-narrow" _builder_version="3.0.92"]

<h3>Before you get started, you'll need the following:</h3>
<ol>
 	<li>You'll need a hosting setup (e.g. at <a href="https://www.bluehost.com/">Bluehost</a>, <a href="https://www.godaddy.com">GoDaddy</a>' etc.).
<ul>
 	<li>There are several different hosts and plans to choose from, so I suggest going with a host that offers a student plan/discount (e.g. like <a href="https://www.bluehost.com/cgi/education">this Bluehost one</a>) or a similarly cheap option (~$5/month). For example, several offer a "shared" hosting plan that comes with the most of the features that you will need: unlimited storage, a free domain name, and the ability to host multiple websites ("addon" domains). Once you pick/purchase a domain name and a hosting plan, be your be sure to note the following information:
<ul>
 	<li><strong>Your FTP address</strong> (e.g. ftp.yourdomain.com)</li>
 	<li><strong>Your Host Username</strong> (e.g. mybluehostusername)</li>
 	<li><strong>Your Host Password</strong> (e.g. chrisisthebest)</li>
</ul>
</li>
</ul>
</li>
 	<li>A FTP (File Transfer Protocol) Application
<ul>
 	<li>Download <a href="https://filezilla-project.org/download.php">Filezilla</a></li>
</ul>
</li>
 	<li>A Code Editor (IDE)
<ul>
 	<li>Download any (or all) of the following:
<ul>
 	<li><a href="https://code.visualstudio.com/">Microsoft Visual Code</a></li>
 	<li><a href="http://brackets.io/">Brackets</a></li>
 	<li><a href="https://atom.io/">Atom</a></li>
 	<li><a href="https://www.sublimetext.com/">Sublime Text</a></li>
</ul>
</li>
</ul>
</li>
</ol>

[/et_pb_text][/et_pb_column][/et_pb_row][/et_pb_section][et_pb_section bb_built="1" module_id="videolesson" _builder_version="3.0.92"][et_pb_row _builder_version="3.0.47" background_size="initial" background_position="top_left" background_repeat="repeat"][et_pb_column type="4_4"][et_pb_text admin_label="Section Heading and Sub-Heading" module_class="text-single-column-narrow" _builder_version="3.0.92"]

<h2>Video Lesson</h2>
<em>Watch the video below for a guided step-by-step demonstration of this assignment. </em>

[/et_pb_text][et_pb_video src="https://www.youtube.com/watch?v=AxCmL9sAlCY" _builder_version="3.0.92" /][/et_pb_column][/et_pb_row][/et_pb_section][et_pb_section bb_built="1" _builder_version="3.0.47"][et_pb_row _builder_version="3.0.47" background_size="initial" background_position="top_left" background_repeat="repeat"][et_pb_column type="4_4"][et_pb_text admin_label="Section Heading and Sub-Heading" module_class="text-single-column-narrow" _builder_version="3.0.92"]

<h2>Setup Your Local Development Environment</h2>
<em>Get setup by creating a root directory for your web site</em>

[/et_pb_text][et_pb_text module_class="text-single-column-narrow" _builder_version="3.0.92"]

<h4>Start by creating a "public_html" folder to act your web site's root directory</h4>
Before you can begin coding, you need to figure out where you are going to work and save your web site's files. A good place would be to set up a root directory somewhere outside of your existing school class folders (where you typically save your class papers, design files, etc). It's a good practice to keep these separate, for many reasons, but one of the most practical reasons is because this assignment (creating a course web site) is not just an assignment for one class (e.g. ART 128) but you are going to set up course web pages for all of your classes (e.g. ART 229). Knowing this, do not place your public_html folder inside of your existing ART128 folder (if you already have one). Instead, keep this up on a higher level.

[/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row _builder_version="3.0.47" background_size="initial" background_position="top_left" background_repeat="repeat"][et_pb_column type="1_2"][et_pb_text admin_label="Image + Caption" _builder_version="3.0.92" text_orientation="center" module_alignment="center"]

<h4>Initial folder setup (as you get started)</h4>
<img class="aligncenter size-full wp-image-1245" src="https://www.creativemedia.space/wp-content/uploads/2018/01/coursewebsite-folderview-step2.gif" alt="" width="1056" height="1003" />

[/et_pb_text][/et_pb_column][et_pb_column type="1_2"][et_pb_text admin_label="Image + Caption" _builder_version="3.0.92" text_orientation="center" module_alignment="center"]

<h4>Final folder setup (once this assignment is completed)</h4>
<img class="aligncenter size-full wp-image-1246" src="https://www.creativemedia.space/wp-content/uploads/2018/01/coursewebsite-folderview-end.gif" alt="" width="1056" height="1003" />

[/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row _builder_version="3.0.47" background_size="initial" background_position="top_left" background_repeat="repeat"][et_pb_column type="4_4"][et_pb_text module_class="text-single-column-narrow" _builder_version="3.0.92"]

<h4>Start with a "base" or "starter" blank HTML page</h4>
Create a new, blank HTML file named index.html and place it in your course directory (e.g. in this case, inside of the art128 folder).

[/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row _builder_version="3.0.47" background_size="initial" background_position="top_left" background_repeat="repeat"][et_pb_column type="4_4"][et_pb_text admin_label="Embedded Gist" _builder_version="3.0.92" text_orientation="center" module_alignment="center"]

[gist https://gist.github.com/kccnma/fa2f9586407d9485ebc8dba98d8b0b2b /]

[/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row _builder_version="3.0.47" background_size="initial" background_position="top_left" background_repeat="repeat"][et_pb_column type="4_4"][et_pb_text module_class="text-single-column-narrow" _builder_version="3.0.92"]

<h4>Add in the content for your course web page.</h4>
Go ahead and add course specific content, such as a link to your first assignment. In this example, for ART 128, add a link to simplewebpage.html. Don't worry about the file not existing yet, because we're going to create that page next.

[/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row _builder_version="3.0.47" background_size="initial" background_position="top_left" background_repeat="repeat"][et_pb_column type="4_4"][et_pb_text admin_label="Embedded Gist" _builder_version="3.0.92" text_orientation="center" module_alignment="center"]

[gist https://gist.github.com/kccnma/ce5583d8e705dd1fcf8456f88eac6eb3 /] Repeat this step for each of your classes so you can post all of your assignments online.

[/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row _builder_version="3.0.47" background_size="initial" background_position="top_left" background_repeat="repeat"][et_pb_column type="4_4"][et_pb_text module_class="text-single-column-narrow" _builder_version="3.0.92"]

<h4>Next, let's create a new HTML file: simplewebpage.html</h4>
[box type="info"] Tip: Resist the temptation to copy-paste the base/starter HTML code to speed up the process. Try writing every line of code from scratch. It's good practice while you learn the basics. [/box]

[/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row _builder_version="3.0.47" background_size="initial" background_position="top_left" background_repeat="repeat"][et_pb_column type="4_4"][et_pb_text admin_label="Embedded Gist" _builder_version="3.0.92" text_orientation="center" module_alignment="center"]

[gist https://gist.github.com/kccnma/607c240aa236f602d6d539d7e2047493 /]

[/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row _builder_version="3.0.47" background_size="initial" background_position="top_left" background_repeat="repeat"][et_pb_column type="4_4"][et_pb_text module_class="text-single-column-narrow" _builder_version="3.0.92"]

<h4>Almost done: Create a Home Page that will link to all of your courses</h4>
Directly inside the root "public_html" level, create another index.html file, but this time, instead of linking to individual course assignments, you are going to link to the individual course web pages (e.g. "art128/index.html").

[/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row _builder_version="3.0.47" background_size="initial" background_position="top_left" background_repeat="repeat"][et_pb_column type="4_4"][et_pb_text admin_label="Embedded Gist" _builder_version="3.0.92" text_orientation="center" module_alignment="center" background_layout="light"]

[gist https://gist.github.com/kccnma/68ce1413705ad92572d9227c2fe2ff12 /]

[/et_pb_text][/et_pb_column][/et_pb_row][et_pb_row _builder_version="3.0.47" background_size="initial" background_position="top_left" background_repeat="repeat"][et_pb_column type="4_4"][et_pb_text module_class="text-single-column-narrow" _builder_version="3.0.92"]

<h4>Last Step: Use Filezilla to upload your site via FTP</h4>
Launch Filezilla and connect to your host (remote) server. To do so, you'll need to enter the domain ftp address and your host username and password. Once you are able to connect successfully, all you need to do is navigate to your target "public_html" or "www" directory and upload your new files and folders. In Filezilla, you can do this by dragging and dropping from the left (local files) to the right (remoter server files).

[/et_pb_text][/et_pb_column][/et_pb_row][/et_pb_section][et_pb_section bb_built="1" _builder_version="3.0.92"][et_pb_row _builder_version="3.0.92"][et_pb_column type="1_4"][/et_pb_column][et_pb_column type="1_2"][et_pb_blurb admin_label="Quick Hands-on Exercise Blurb" title="Nice Work!" use_icon="on" font_icon="%%57%%" icon_color="#000000" use_icon_font_size="on" icon_font_size="32px" _builder_version="3.0.92" text_orientation="center" url_new_window="off" use_circle="off" use_circle_border="off" icon_placement="top" background_layout="light"]

If you completed this assignment, great job!

[/et_pb_blurb][/et_pb_column][et_pb_column type="1_4"][/et_pb_column][/et_pb_row][/et_pb_section][et_pb_section bb_built="1" _builder_version="3.0.47"][et_pb_row _builder_version="3.0.47" background_size="initial" background_position="top_left" background_repeat="repeat"][et_pb_column type="4_4"][et_pb_text admin_label="Conclusion" module_class="text-single-column-narrow" _builder_version="3.0.92"]

<h2>Conclusion</h2>
Getting started with front-end web development can be the hardest step. The good news is that once you get setup, it gets easier and easier for you to practice writing code and building web sites.

[/et_pb_text][/et_pb_column][/et_pb_row][/et_pb_section]