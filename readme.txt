=== Elokenz - Author's Most Shared Articles ===
Contributors: tanzaho, juliobox
Donate link: http://www.elokenz.com
Tags: social, share, sharing, seo, smo, facebook, twitter, google+, retweet, Post, widget, sidebar, authorship 
Requires at least: 3.1
Tested up to: 3.8
Stable tag: 2.0.3
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Widget for bloggers using "authorship" attribution. Show your readers your best articles, wherever they are written..

== Description ==

If you are tagging your articles with the "<a href="https://plus.google.com/authorship">authorship</a>" markup from Google+, and want to collect your best articles from around the web (from all your blogs), this plugin is made for you.

You will be able to collect and show the number of mentions from Twitter, Facebook and Google+ for all your articles and display the top 5. You can also use the widget for multi-authors blogs.

Before using the plugin, you must make sure that you have some articles associated to your google+ author profile. In order to do that, log into <a href="http://www.elokenz.com">Elokenz.com</a> and wait until our bot visits your websites. This takes in general less than 5 minutes.


== Installation ==

= How to install Elokenz widget sitewide ? =
This section describes how to install the plugin and get the widget working sitewide (in your sidebar). If you want to use the plugin on a unique page, please read below.

* Step 1. Upload the plugin to `/wp-content/plugins/` directory
* Step 2. Activate the plugin through the 'Plugins' menu in WordPress
* Step 3. Create an account on http://www.elokenz.com (needed to import your data)
* Step 4. Create a new widget from the 'Appearance' page : `/wp-admin/widgets.php`
* Step 5. Fill-out the widget with your Google+ id
* Step 6. Change the settings of the plugin (width, number of items, theme)

= How to use Elokenz widget on a page/post ? =
In order to add the widget in a page/post (and not in the sidebar), you can use a `shortcode`. For that, you can add the following text when you are editing an article :

`[elokenz_widget user_id="113400244614302404694"]` (where `113400244614302404694` is replaced by your Google+ id).
 
You can use several **arguments** to configure the output :
* width [integer] : give the width in pixel. (Default : the widget will use all available space)
* follow ["do"/"no"] :  use dofollow links or nofollow links. (Default : dofollow links)
* style ["bright"/"dark"] : use a bright or dark background. (Default : "bright")
* item_number [integer < 10] : how many articles do you want to list here ? (Default : 5)
* network [0,1,2 or 3] : which ordering system should we use ? (Default : 0)
    0. sum of all metrics
    1. Twitter
    2. Facebook
    3. Google+ 

**Example** :
  `[elokenz_widget user_id="113400244614302404694" follow="no" item_number="10"  style="dark" network="1"]`      
  will output a list of 10 articles, with nofollow links, on a dark background, order according the number of RTs.

== Frequently Asked Questions ==

= Which social metric do I see ? =

At the moment, we show only the number of facebook likes, the number of retweets and the number of Google+ +1. The list might be extended in the future.

= Can I add special social networks metrics? =

This will be done in the future releases.

= Where can I find my Google+ id ? =

Visit your Google+ profile page (https://plus.google.com/u/0/me?tab=XX) and pass the mouse over your name. 
There should be a link with several digits like : https://plus.google.com/113400244614302404694 . Your google+ id should be : 113400244614302404694

Alternatively, you can also log into your Elokenz profile and check your settings : http://www.elokenz.com/dashboard/settings/

= External resources =

Here are listed some external resources to get you started with the plugin. 
French : http://www.tendances-webmarketing.com/2014/02/plugin-wordiz-wordpress-top-blog-posts-partages-reseaux-sociaux.html


= Can I contribute to this 'wonderful' plugin? =

Of course and you are welcome. The code will soon be posted on Github. 
You can also rate the plugin if you like it.


== Screenshots ==

1. This is what you will see with the bright theme.
2. This is what you will see with the dark theme.
3. This is the widget settings in Wordpress administration. 
4. Output from the widget. Several domains can be listed in function of your articles.

== Changelog ==

= 2.0.3 =
* Added missing CSS

= 2.0.2 =
* Added shortcode support

= 2.0.1 =
* Fixed a bug with the cache which prevented regular updates of your social share counts
* Added an option for the ranking system (Total, Twitter, Facebook or Google+)
* Changed name of plugin (old wordiz becomes elokenz)

= 1.0.5 =
* Added a sign in button directly in the widget options

= 1.0.4 =
* Fixed CSS width (fixed -> auto)
* Removed ability to change width
* Adjusted space between social media icons

= 1.0.3 =
* Fixed CSS conflict with other widgets.
* Fixed Google+ count import
* Todo : Fix width not working properly

= 1.0.2 =
* Added a better help in the widget panel
= 1.0.1 =
* Added some description
= 1.0 =
* First upload of the plugin