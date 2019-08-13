---
ID: 1948
post_title: Intro to CMS via WordPress
author: CMS
post_excerpt: ""
layout: post
permalink: >
  https://creativemedia.space/intro-to-cms-via-wordpress/
published: true
post_date: 2018-08-19 17:31:36
---
<!-- wp:paragraph -->
<p>One of the best ways to learn about content management systems (CMS) is to set one up from scratch. In this lesson, we are going to use <a href="https://wordpress.org/">Wordpress</a> to set up a small, simple CMS-driven "test" web site for learning purposes.</p>
<!-- /wp:paragraph -->

<!-- wp:quote -->
<blockquote class="wp-block-quote"><p>A <strong>Content Management System</strong>&nbsp;(CMS) is a computer application that supports the creation and modification of digital content. It is typically used to support multiple users working in a collaborative environment. Most CMSs include Web-based publishing, format management, history editing and version control, indexing, search, and retrieval. By their nature, content management systems support the separation of content and presentation.<br> – <a href="https://en.wikipedia.org/wiki/Content_management_system">Wikipedia</a></p></blockquote>
<!-- /wp:quote -->

<!-- wp:quote -->
<blockquote class="wp-block-quote"><p><strong>WordPress</strong> is a free and open-source content management system (CMS) based on PHP and MySQL.<br> – <a href="https://en.wikipedia.org/wiki/WordPress">Wikipedia</a></p></blockquote>
<!-- /wp:quote -->

<!-- wp:heading {"level":4} -->
<h4>Outcomes:</h4>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li>Learn how to:
<ul><li>Install &amp; Setup a CMS (Wordpress) - <a href="http://www.egargiulo.com/nma/test01/">Example</a></li><li>Add/Manage Content (using Wordpress's admin interface)</li><li>Customize the visual style (via Wordpress themes) in different ways:
<ul><li>Modify an existing theme</li><li>Upload a custom theme - <a href="http://www.egargiulo.com/nma/test07/">Example</a></li></ul>
</li></ul>
</li></ul>
<!-- /wp:list -->

<!-- wp:heading {"level":4} -->
<h4>Related Concepts</h4>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li>Templating</li><li>Separating Content &amp; Presentation</li></ul>
<!-- /wp:list -->

<!-- wp:heading {"level":4} -->
<h4>Related Reading &amp; Resources</h4>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li><a href="https://wordpress.org/">Wordpress.org</a></li><li><a href="https://wordpress.com/">Wordpress.com</a></li></ul>
<!-- /wp:list -->

<!-- wp:separator -->
<hr class="wp-block-separator"/>
<!-- /wp:separator -->

<!-- wp:heading -->
<h2>Install and Setup Wordpress</h2>
<!-- /wp:heading -->

<!-- wp:list {"ordered":true} -->
<ol><li>Install Wordpress
<ul><li>Login to your host &gt; cpanel &gt; &nbsp;install wordpress in a sub-directory
<ul><li>Example: <a href="http://www.egargiulo.com/nma/test01/">/Test01/</a></li><li>Be sure to note your site's login credentials</li></ul>
</li></ul>
</li><li>Setup Wordpress
<ul><li>Adjust the Settings for a small site
<ul><li>Login to your site's dashboard/admin
<ul><li>yourdomain.com/test01/wp-admin</li></ul>
</li><li>&gt; Plugins
<ul><li>&gt; Installed Plugins: deactivate and delete default plugins that will not be needed
<ul><li>Some examples to remove (from Bluehost's default install): Google Analytics for WordPress by MonsterInsights, Hello Dolly, MOJO Marketplace, OptinMonster, WPForms Lite</li><li>Be sure to keep:&nbsp; Akismet Anti-Spam and JetPack</li></ul>
</li></ul>
</li><li>&gt; Settings
<ul><li>&gt; Discussion: Turn off comments</li></ul>
</li></ul>
</li></ul>
</li></ol>
<!-- /wp:list -->

<!-- wp:separator -->
<hr class="wp-block-separator"/>
<!-- /wp:separator -->

<!-- wp:heading -->
<h2>Add Initial Content in Wordpress</h2>
<!-- /wp:heading -->

<!-- wp:list {"ordered":true} -->
<ol><li>Add Content
<ul><li>&gt; Pages
<ul><li>Delete default/existing pages</li><li>Create a new page titled "Home"</li><li>Create a new page title "Sub Page"
<ul><li>For content, use <a href="https://gist.githubusercontent.com/kccnma/7ea4822437a69a61c3fa26533cb5f1ef/raw/08ee13f3c09ca849f99fbfc07e00ece8217145d3/base-typography-content.html">base content/typography markup (raw html)</a></li></ul>
</li></ul>
</li><li>&gt; Settings
<ul><li>&gt; Reading: Set the Front Page to display your newly created "Home" page</li></ul>
</li><li>&gt; Appearance
<ul><li>&gt; Menus: Create a new Menu (e.g. "Main Menu") and set it's location as the Primary Menu</li></ul>
</li></ul>
</li></ol>
<!-- /wp:list -->

<!-- wp:heading -->
<h2>Customize Your Wordpress Site</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>There are many different ways to customize a WP site, below are are few known techniques that you should be familiar with as you consider your best options per project:</p>
<!-- /wp:paragraph -->

<!-- wp:list -->
<ul><li>You can customize a theme via Customizer <ul><li>Appearance > Customize <ul><li>Browse the built-in theme settings and experiment with the theme-supported settings</li></ul></li></ul></li><li>You can change the Theme <ul><li>Appearance > Themes > Add New<ul><li>Search or browse for a new third-party theme </li></ul></li></ul></li><li>You can modify a Theme<ul><li>Manually edit a theme's css and php files directly via Appearance > Editor <em>(not recommended*)</em></li><li>Manually edit a theme's css and php files locally then update/upload via FTP <em>(not recommended*)</em></li></ul></li><li>You can create a Child Theme  <ul><li>Create a new theme directory with only the files that you want to override <em>(highly recommended)</em></li></ul></li><li>You can create your own Custom Theme<ul><li>This option provides the most control, but it also the most costly in terms of development time <em>(advanced, but highly recommended)</em></li></ul></li></ul>
<!-- /wp:list -->

<!-- wp:paragraph -->
<p><em>* It is never recommended to edit a found parent theme's files because all changes/modifications will be lost if/when the theme is updated. A safer approach is to use a child theme or to create a custom parent theme.</em></p>
<!-- /wp:paragraph -->

<!-- wp:separator -->
<hr class="wp-block-separator"/>
<!-- /wp:separator -->

<!-- wp:heading -->
<h2>Conclusion &amp; Resources</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Wordpress is a powerful content management system, but one of the main challenges faced by web designers and developers is figuring out how to best customize WP sites based upon client goals, needs, budgets, and scopes for different projects. Below are some customization techniques to consider, starting from easiest (and least customizable) to the hardest (yet most customizable):</p>
<!-- /wp:paragraph -->

<!-- wp:list {"ordered":true} -->
<ol><li><strong>Customize an Existing or Default Theme</strong> (e.g. WP default themes)<ul><li>Use the built-in "Customizer" tool via the admin interface and adjust your theme's built-in settings</li><li>Override their settings via "Additional CSS" in the admin interface <em>(not recommended* for production, but might be justified in certain use cases, such as working with a client with no FTP access and/or no child theme option)</em></li><li>Manually edit a theme's files (e.g. style.css) locally then update/upload via FTP <em>(not recommended*)</em></li></ul></li><li><strong>Switch to a New Third-Party Theme</strong> (<em>Free</em> or <em>Paid</em>)<ul><li>Choose from the many existing free themes available (e.g. <a href="https://wpastra.com/">Astra</a>)</li><li>Purchase a premium theme (e.g. <a href="https://wpastra.com/pro/">Astra Pro</a>, <a href="https://www.elegantthemes.com/gallery/divi/">Divi</a>) </li></ul></li><li><strong>Child Theme an Existing Parent Theme</strong> <ul><li>Create a custom child theme that will manually override the parent theme settings a-la-carte. (e.g. Astra, Divi, etc—or any fully featured theme with the desired features and functionality already built-in) </li><li>Child Theme Resources: <ul><li><a href="https://codex.wordpress.org/Child_Themes">Wordpress Codex: Child Themes</a></li></ul></li><li>Child Theme Examples: <ul><li><a href="https://woocommerce.com/">WooCommerce</a> > <a href="https://woocommerce.com/storefront/">Storefront</a> > Storefront Child Theme</li><li><a href="https://github.com/kccnma/teachingmaterials/tree/master/mychildtheme-wp">Chris's "My Child Theme WP"</a> (A blank Child Theme) <ul><li>Download: <a href="https://github.com/kccnma/teachingmaterials/raw/master/mychildtheme-wp.zip">mychildtheme-wp.zip </a></li></ul></li><li>NOTE: Be sure to change the parent theme name in style.css </li></ul></li></ul></li><li><strong>Create Your Own Custom Theme</strong> <ul><li>Start with a "starter" theme framework (e.g. <a href="https://underscores.me/">_underscores</a>)</li></ul><ul><li>Code a theme from scratch (starting with the core essentials: index.php, style.css, &amp; screenshot.png) <ul><li>Example: Chris's <a href="http://www.egargiulo.com/nma/test07/">Sitebase-wp</a> </li></ul></li></ul></li><li><strong>Use 3rd Party Plugins</strong> <ul><li>Extend/Customize your base theme's built-in features and functionality by installing third-party plugins<ul><li>For example, for more layout control consider using a Page Builder plugin like <a href="https://siteorigin.com/page-builder/">Site Origins Page Builder</a>, <a href="https://elementor.com/">Elementor</a>, <a href="https://www.wpbeaverbuilder.com/">Beaver</a> etc.</li><li>Popular Plugins to consider:<ul><li>ACF (Advanced Custom Fields)</li><li>CPT UI (Custom Post Types UI)</li><li>Helpful Shortcode plugins:<ul><li>Display Posts</li><li>Insert Pages</li></ul></li></ul></li></ul></li></ul></li></ol>
<!-- /wp:list -->