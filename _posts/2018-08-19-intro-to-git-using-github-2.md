---
ID: 1942
post_title: Intro to Git using Github
author: Front-end Freddy
post_excerpt: ""
layout: post
permalink: >
  https://creativemedia.space/intro-to-git-using-github-2/
published: true
post_date: 2018-08-19 17:25:39
---
<!-- wp:heading {"level":3} -->
<h3>A Version Control Workflow</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>In this lesson, we will learn about <a href="https://git-scm.com/">Git</a> via a hands-on exercise using <a href="https://github.com/">Github</a><a href="https://github.com/">.</a></p>
<!-- /wp:paragraph -->

<!-- wp:quote -->
<blockquote class="wp-block-quote"><p><strong>Git</strong> is a version control system for tracking changes in computer files and coordinating work on those files among multiple people.<br> – <a href="https://en.wikipedia.org/wiki/Git">Wikipedia</a></p></blockquote>
<!-- /wp:quote -->

<!-- wp:quote -->
<blockquote class="wp-block-quote"><p><strong>GitHub</strong> is a web-based Git or version control repository and Internet hosting service. It is mostly used for code. It offers all of the distributed version control and source code management (SCM) functionality of Git as well as adding its own features. It provides access control and several collaboration features such as bug tracking, feature requests, task management, and wikis for every project.<br> – <a href="https://en.wikipedia.org/wiki/GitHub">Wikipedia</a></p></blockquote>
<!-- /wp:quote -->

<!-- wp:paragraph -->
<p>Git is a “distributed” version control system, where you keep your code in one place and are able to manage, track, and backup your code (e.g. using GitHub, a hosting platform that uses Git). It can be complex, especially when it comes to managing large projects with large teams. In this lesson, we are going to cover the basics specifically geared toward individual web designers, front-end developers and small teams working on small projects.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>Outcomes:</h4>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li>Learn the basics of Git and common git commands via CLI (Command Line Interface)</li><li>Learn how to install Git locally, setup your local environment, and create a new repository from scratch.</li><li>Learn a basic daily workflow of syncing a local repository with a remote repository on GitHub, editing it locally, and updating it.</li></ul>
<!-- /wp:list -->

<!-- wp:heading {"level":4} -->
<h4>Lesson Resources:</h4>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li><a href="https://github.com/johndoenma/hello-world">Hello World</a> (a first repository, for learning purposes)</li></ul>
<!-- /wp:list -->

<!-- wp:heading {"level":4} -->
<h4>Steps:</h4>
<!-- /wp:heading -->

<!-- wp:list {"ordered":true} -->
<ol><li><strong>Install Git</strong><br><em>Make sure that you have Git installed on your local machine</em></li><li><strong>Setup a Repo</strong><br><em>Create your first repository on Github from scratch</em></li><li><strong>Daily Git Workflows</strong><br><em>Update an existing repository on Github</em></li></ol>
<!-- /wp:list -->

<!-- wp:image {"linkDestination":"custom"} -->
<figure class="wp-block-image"><img src="https://imgs.xkcd.com/comics/git_2x.png" alt="Git Comic"/><figcaption>Git comic from <a href="https://xkcd.com/1597/">xkcd</a></figcaption></figure>
<!-- /wp:image -->

<!-- wp:separator -->
<hr class="wp-block-separator"/>
<!-- /wp:separator -->

<!-- wp:spacer -->
<div style="height:100px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:spacer -->

<!-- wp:uagb/advanced-heading {"block_id":"c20ca385-beb4-4e1d-9a97-35ce92947424","className":"step-heading"} -->
<div class="wp-block-uagb-advanced-heading step-heading" id="uagb-adv-heading-c20ca385-beb4-4e1d-9a97-35ce92947424"><h2 class="uagb-heading-text">Part</h2><div class="uagb-separator-wrap"><div class="uagb-separator"></div></div><p class="uagb-desc-text">1</p></div>
<!-- /wp:uagb/advanced-heading -->

<!-- wp:heading -->
<h2>Install Git</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><em>Make sure that you have Git installed on your local machine</em></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Before you install anything, first check to see if you have it already installed. You can confirm via the following commands (to be entered via CLI, such as Terminal on a MAC or Command Prompt on a PC)</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code lang="bash" class="language-bash">$ git --version</code></pre>
<!-- /wp:code -->

<!-- wp:list {"ordered":true} -->
<ol><li>If you already have git installed, move on to Step #2. If you do not have git installed, follow the <a href="https://git-scm.com/book/en/v2/Getting-Started-Installing-Git">installation instructions on the Git web site</a>.
<ul><li>Another option: you can also download&nbsp;<a href="https://desktop.github.com/">GitHub Desktop</a>, a GUI client, that will automatically install git on your computer. However, I do not recommend using GitHUb Desktop to learn Git. Instead, I recommend using the command line interface (CLI), which we will do in this lesson.</li></ul>
</li></ol>
<!-- /wp:list -->

<!-- wp:separator -->
<hr class="wp-block-separator"/>
<!-- /wp:separator -->

<!-- wp:spacer -->
<div style="height:100px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:spacer -->

<!-- wp:uagb/advanced-heading {"block_id":"3a92800d-693e-477b-b0c8-d15b797b711c","className":"step-heading"} -->
<div class="wp-block-uagb-advanced-heading step-heading" id="uagb-adv-heading-3a92800d-693e-477b-b0c8-d15b797b711c"><h2 class="uagb-heading-text">Part</h2><div class="uagb-separator-wrap"><div class="uagb-separator"></div></div><p class="uagb-desc-text">2</p></div>
<!-- /wp:uagb/advanced-heading -->

<!-- wp:heading -->
<h2>Get Setup on GitHub</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><em>Create your first repository on Github from scratch</em></p>
<!-- /wp:paragraph -->

<!-- wp:list -->
<ul><li>Create an account at <a href="https://github.com/">Github.com</a> and log in.
<ul><li>Note your user name</li><li>Note your user email address</li></ul>
</li><li>Configure your git username and email address to match your github account (e.g. if you are using github).</li></ul>
<!-- /wp:list -->

<!-- wp:code -->
<pre class="wp-block-code"><code lang="bash" class="language-bash">$ git config --global user.name "John Doe"
$ git config --global user.email johndoe@example.com</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>To test/ensure that your username and email configurations are correct:</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code lang="bash" class="language-bash">$ git config --global user.name
$ git config --global user.email</code></pre>
<!-- /wp:code -->

<!-- wp:list -->
<ul><li>Create a repository<br>A repository is essentially a main project folder, designed to organize single projects. Each can contain multiple sub folders and files. All repositories should have a README, a default file for each repository with information about the project. GitHub makes it easy to add one whenever you create a new repository using your browser (via github.com). It also offers other common options such as adding a .gitignore file (which some beginners find challenging to to create locally) along with license options.
&nbsp;
<ol><li>In the upper right corner, click + and then select "New Repository"</li><li>Name your repository “hello-world”</li><li>Write a short description</li><li>Select Initialize this repository with a README</li></ol>
</li></ul>
<!-- /wp:list -->

<!-- wp:separator -->
<hr class="wp-block-separator"/>
<!-- /wp:separator -->

<!-- wp:spacer -->
<div style="height:100px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:spacer -->

<!-- wp:uagb/advanced-heading {"block_id":"f0da8e9b-d9b3-4137-814f-fca0be6042c8","className":"step-heading"} -->
<div class="wp-block-uagb-advanced-heading step-heading" id="uagb-adv-heading-f0da8e9b-d9b3-4137-814f-fca0be6042c8"><h2 class="uagb-heading-text">Part</h2><div class="uagb-separator-wrap"><div class="uagb-separator"></div></div><p class="uagb-desc-text">4</p></div>
<!-- /wp:uagb/advanced-heading -->

<!-- wp:heading -->
<h2>Daily Git Workflows</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><em>Use Git (e.g. GitHub) as part of your daily practice</em></p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>#1 Daily Workflow for a <strong>New</strong> Project</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><em> (if this is your first time working on locally, or you previously deleted your local folder and need to set it up again)</em><br>Via command line, navigate to your a target parent directory</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code lang="bash" class="language-bash">$ cd targetparentdirectory</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Confirm that you are in the right place by listing the directory files/folders</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code lang="bash" class="language-bash">$ ls -l // for Mac users
$ dir // for PC users</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Clone the directory to your repo on github (tip: copy/paste the url path to the repo via your browser, e.g. https://github.com/username/reponame/)</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code lang="bash" class="language-bash">$ git clone &lt;path-to-repository></code></pre>
<!-- /wp:code -->

<!-- wp:code -->
<pre class="wp-block-code"><code lang="bash" class="language-bash">// Example:
// $ git clone https://github.com/johndoenma/hello-world</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Once the repo is cloned to your local machine, you'll need to navigate into the project folder/directory</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code lang="bash" class="language-bash">$ cd projectfolder</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Once again, you can confirm that you are in the right place by listing the directory files/folders</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code lang="bash" class="language-bash">$ ls -l // for Mac users
$ dir // for PC users</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Optional/additional confirmation: at any time you can double-check the status of your repo to see if your cloned local repo is up-to-date</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code lang="bash" class="language-bash">$ git status</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>You are set to begin editing! (e.g. edit the README.md file, add project folders or files, run gulp, edit/code, etc).</p>
<!-- /wp:paragraph -->

<!-- wp:list -->
<ul><li>For this initial "hello world" lesson, open your IDE (editor of choice) and edit the README.md file, then save it.</li><li>After you have made a change to your README.md file, move on the the Daily Workflow steps below for <em>when you are done for the day</em>.</li></ul>
<!-- /wp:list -->

<!-- wp:heading {"level":4} -->
<h4>#2 Daily Workflow for an <strong>Existing</strong> Project</h4>
<!-- /wp:heading -->

<!-- wp:heading {"level":6} -->
<h6><em>(if you already have a project setup and worked on it locally before)</em></h6>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Via command line, navigate to your a target parent directory</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code lang="bash" class="language-bash">$ cd projectfolder</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Check the status of your repo to see if your cloned local repo is up-to-date</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code lang="bash" class="language-bash">$ git status</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>If your local folder is up-to-date, then you are set to go! (e.g. edit files, run gulp, etc.)</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>If your local folder is not up-to-date, then you need to update your local repo to match the remote repo by "pulling" the latest version.</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code lang="bash" class="language-bash">$ git pull</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>To confirm that your pull worked, you can double-check the status of your repo to see if your cloned local repo is now up-to-date</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code lang="bash" class="language-bash">$ git status</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>You are set to go! (e.g. edit files, run gulp, etc.)</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>#3 Daily Workflow for <strong>When You are Done for the Day</strong></h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><em>(you should memorize these commonly used git commands)</em></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>When you are done editing for the day, the following are the most commonly used git commands for solo developers.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>First off, whenever you are done for the day, you should always check the status of your repo before you commit.</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code lang="bash" class="language-bash">$ git status</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>If your local version is ahead of master (which it should be if you are a solo developer), then these three commands will be the most important ones to memorize:</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code lang="bash" class="language-bash">$ git add -A
$ git commit -m “comment goes here”
$ git push origin master</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>If successful (e.g. no errors), you should be able to double-check by launching your browser and viewing your github.com repository to ensure that all recent updates/changes have been uploaded to github.com.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Congratulations, you are now up and running on github!</p>
<!-- /wp:paragraph -->

<!-- wp:separator -->
<hr class="wp-block-separator"/>
<!-- /wp:separator -->

<!-- wp:heading {"level":3} -->
<h3>Further Reading</h3>
<!-- /wp:heading -->

<!-- wp:heading {"level":4} -->
<h4>Git Related Reading and Learning Resources</h4>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li><a href="https://try.github.io/levels/1/challenges/1">GitHub's Interactive Learning Guide</a> (Intro to Git)</li><li><a href="https://guides.github.com/activities/hello-world/">GitHub's Hello World Guide</a> (Intro using Branching)</li><li><a href="https://help.github.com/">GitHub's Help Documentation</a></li><li><a href="https://www.youtube.com/githubguides">GitHub's Video Learning Guides</a></li><li><a href="https://services.github.com/on-demand/downloads/github-git-cheat-sheet.pdf">GitHub's Cheat Sheet</a> (pdf)</li><li><a href="https://git-scm.com/docs">Git's Docs</a> (Cheat Sheet)</li><li><a href="https://www.atlassian.com/git">Atlassian's Getting Git Right</a> (Workflow Example)</li></ul>
<!-- /wp:list -->