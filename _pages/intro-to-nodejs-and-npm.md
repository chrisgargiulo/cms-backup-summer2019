---
ID: 588
post_title: Intro to Node.js and npm
author: CMS
post_excerpt: ""
layout: page
permalink: >
  https://creativemedia.space/lessons/intro-to-nodejs-and-npm/
published: true
post_date: 2017-10-31 01:03:24
---
<!-- wp:heading {"level":3} -->
<h3>Package Management using npm</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>In this lesson, we will learn how to use the package manager <a href="https://www.npmjs.com/">npm</a>, a <a href="https://nodejs.org/en/">node.js</a> command line client, to setup a custom front-end web development environment and automated build process.</p>
<!-- /wp:paragraph -->

<!-- wp:quote -->
<blockquote class="wp-block-quote"><p>A <strong>package manager</strong> (or package management system) is a collection of tools that automates the process of installing, upgrading, configuring, and removing software in a consistent manner.<br> – <a href="https://en.wikipedia.org/wiki/Package_manager">Wikipedia</a></p></blockquote>
<!-- /wp:quote -->

<!-- wp:quote -->
<blockquote class="wp-block-quote"><p><strong>npm</strong> is a package manager for the JavaScript programming language. It is the default package manager for the JavaScript runtime environment Node.js. It consists of a command line client, also called npm, and an online database of public and paid-for private packages, called the npm registry. The registry is accessed via the client, and the available packages can be browsed and searched via the npm website. The package manager and the registry are managed by npm, Inc.<br> – <a href="https://en.wikipedia.org/wiki/Npm_(software)">Wikipedia</a></p></blockquote>
<!-- /wp:quote -->

<!-- wp:quote -->
<blockquote class="wp-block-quote"><p><strong>Node.js</strong> is an open-source, cross-platform JavaScript run-time environment for executing JavaScript code server-side. Historically, JavaScript was used primarily for client-side scripting, in which scripts written in JavaScript are embedded in a webpage's HTML, to be run client-side by a JavaScript engine in the user's web browser. Node.js enables JavaScript to be used for server-side scripting, and runs scripts server-side to produce dynamic web page content before the page is sent to the user's web browser. Consequently, Node.js has become one of the foundational elements of the "JavaScript everywhere" paradigm, allowing web application development to unify around a single programming language, rather than rely on a different language for writing server side scripts.<br> – <a href="https://en.wikipedia.org/wiki/Node.js">Wikipedia</a></p></blockquote>
<!-- /wp:quote -->

<!-- wp:heading {"level":4} -->
<h4>Why use a package manager like npm?</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>As front-end web development environments and build tools become more and more complex, the amount of time spent setting up new projects can be exhaustive. To avoid wasting time via repetition, package managers help to simplify the process with one simple command: <code>npm install</code>.</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>$ npm install
</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Package managers like npm can save front-end developers a lot of time, especially when starting new projects from scratch (e.g. to avoid setting up everything manually), when working with complex projects with multiple dependencies (e.g. to avoid installing each dependency with the latest version of each), and when working on large projects with multiple developers (to ensure a consistency across all computers).</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>Outcomes</h4>
<!-- /wp:heading -->

<!-- wp:list {"ordered":true} -->
<ol><li>Learn how to install an existing npm-based web project</li><li>Learn how to setup a custom npm-based web project from scratch</li></ol>
<!-- /wp:list -->

<!-- wp:heading {"level":4} -->
<h4>Steps</h4>
<!-- /wp:heading -->

<!-- wp:list {"ordered":true} -->
<ol><li>Install Node.js and npm</li><li>Install an existing npm project (Sitebase 3)</li><li>Setup a custom npm project from scratch (my-npm-project)</li></ol>
<!-- /wp:list -->

<!-- wp:separator -->
<hr class="wp-block-separator"/>
<!-- /wp:separator -->

<!-- wp:heading -->
<h2>Step 1</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><em>Install Node.js and npm</em></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Make sure that you have node.js installed.</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>$ node -v
$ npm -v
</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>If installed, you should see the version number for each. If not, you'll need to download Node.js from <a href="https://nodejs.org/en/">https://nodejs.org/en/</a> and follow their installation instructions.</p>
<!-- /wp:paragraph -->

<!-- wp:separator -->
<hr class="wp-block-separator"/>
<!-- /wp:separator -->

<!-- wp:heading -->
<h2>Step 2</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><em>Install an existing npm project: Sitebase 3</em></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Inside of your target parent directory (the folder where you will be placing your new project folder), copy the source project files for <a href="https://github.com/kccnma/sitebase3-npmgulp">Sitebase 3.0 on Github</a>. If you already have git installed and/or already have a github account, from inside of your target parent directory, you can simply clone the repo:</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>$ git clone https://github.com/kccnma/sitebase3-npmgulp
</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>If you do not have git installed, you can download the zip file (<a href="https://github.com/kccnma/sitebase3-npmgulp/archive/master.zip">https://github.com/kccnma/sitebase3-npmgulp/archive/master.zip</a>) then manually unzip it into your target parent directory.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Once copied/cloned, your local environment should look like this:</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>targetparentdirectory/
   └── sitebase3-npmgulp/
         ├── dist/
         ├── src/
         ├── .gitignore
         ├── README.md
         ├── gulpfile.js
         ├── package.json
</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Take a look inside of <strong>package.json</strong> and you'll notice two sections toward the bottom: <em>dependencies</em> and <em>devDependencies</em>. These are the list of dependencies that this existing project is already using. In this case, this project is using gulp as a task manager to watch for changes, compile source files (e.g. SASS via a gulp plugin called gulp-sass), sync browsers (via browser-sync), compress all images (via gulp-imagemin), and then compile and copy all final files into the <strong>/dist/</strong> folder.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3>Testing</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>If you try to run <code>gulp</code> right away, it will not work. You'll get an error (e.g. <code>"Local gulp not found"</code>). The key step (whenever you are setting up a new project via npm) is to run <code>npm install</code> from inside of your project folder <em>first</em>. Note: you only need to do this <em>once</em>.</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>$ cd sitebase3-npmgulp
$ npm install
</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>You'll notice a progress bar as npm installs all of the project dependencies. Afterward, you'll notice a new folder was created entitled <strong>"node_modules"</strong> that contains all of the dependencies. Note: this <strong>"node_modules"</strong> folder is quite large, so if you are using git, be sure to add it to your <strong>.gitignore</strong> file (which is already included as part of Sitebase 3).</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>To test it out, run <code>gulp</code> and see if it works. It should spin up a web server, launch the project in a browser, and watch your files for changes.</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>$ gulp
</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Congratulations - you just setup your first npm-based web project!</p>
<!-- /wp:paragraph -->

<!-- wp:separator -->
<hr class="wp-block-separator"/>
<!-- /wp:separator -->

<!-- wp:heading -->
<h2>Step 3 <em>(Optional)</em></h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><em>Advanced: Setup a custom npm project from scratch (my-npm-project)</em></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Let's say you do not want to start from an existing project or base, and would prefer to setup a completely new npm-based project from scratch. The steps are simple:</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3>npm init</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>First, wherever you are working (e.g. your target parent folder), create a new primary "projectname" folder to be the project root directory. Then, run the <code>npm init</code> command from inside your target parent directory.</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>$ npm init
</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>The <code>npm init</code> command will create a <strong>package.json</strong> file that will store information about the project, such as the dependencies used in the project (e.g. Gulp, Sass, etc.) and it will also create a new <strong>"node_modules"</strong> folder that will include all dependencies. In order to create the <strong>package.json</strong> file with accurate information, it will prompt you <code>"Is this ok? (yes)?</code> Type <code>yes</code>.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>If you look inside of your project folder, you should see both the new <strong>package.json</strong> file and the new <strong>node_modules</strong> folder.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3>Add Dependencies</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Once you have your <strong>package.json</strong> file all set up and ready, whenever you need to add a new dependency to your project, you'll need to 1) manually install each dependency and 2) save it to your list of dependencies inside of your project's <strong>package.json</strong> file. This two-part process is actually quite simple and done in one step via the following command:</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>$ npm install dependencyname --save-dev (replacing dependencyname with the name of your dependency)
</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Be sure to include the <code><strong>"--save-dev"</strong></code> part, or else the dependency will not be added to your list of dependencies inside of your project's <strong>package.json</strong> file. As an example, let's install gulp.</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>$ npm install gulp --save-dev
</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>If you look inside of your <strong>package.json</strong> file, you should see "gulp" along with the version number inside of the "devDependencies" area.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Since this lesson is about npm (not gulp), we are not going to create a complex <strong>gulpfile.js</strong>. However, we can setup a quick one to test that our custom environment is working OK.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>First, we'll need to create a new file named <strong>"gulpfile.js"</strong> that will store all of your gulp tasks. I suggest using your favorite text editor (IDE) for this step. Inside of your <strong>gulpfile.js</strong>, we'll need to add a task for testing purposes. Whenever you add a new task using gulp, such as adding a new dependency, it is a 2-step process:</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>1) First, you need to add a "require" statement that will tell Node to look into the node_modules folder for the new package (in this case it is a package named gulp). To do this, you need to create a new variable named <code>gulp</code> and assign the plugin contents to it:</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>var gulp = require('gulp');
</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>2) Next, you need to define the task. The following is the syntax for a typical gulp task:</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>gulp.task('task-name', function() {
    // Statements go here
});
</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>In this case, we are going to do a simple "Hello" console log statement to a task named hello.</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>gulp.task('hello', function() {
    console.log('Hello');
});
</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>After you saved your gulpfile from your text editor, switch to your command line interface and test it out via the following command:</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>$ gulp hello
</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Congratulations! You just created a custom npm-project!</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2>Closing thoughts:</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Project managers can speed up the setup and installation of project dependencies, build tools, and processes. Once you have npm installed on your machine, you can quickly and easily take advantage of existing npm-based projects that use npm install for project setup and the many npm packages and dependencies that it supports.</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2>Resources:</h2>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li>Node.js - <a href="https://nodejs.org/en/">https://nodejs.org/en/</a></li><li>npm - <a href="https://www.npmjs.com/">https://www.npmjs.com/</a></li></ul>
<!-- /wp:list -->