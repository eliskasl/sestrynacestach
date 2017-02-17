=== Google Photos WordPress Plugin ===

Contributors: nakunakifi
Donate link: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=ZAZHU9ERY8W34
Tags: album, albums, CDN, google picasa, image, images gallery, image hosting, lightbox, picasa, picasa web, photo, photos, google photos, photo albums, showcase
Requires at least: 3.0.1
Tested up to: 4.7
Stable tag: 3.0.9

Display Google Photo & Google Picasa Albums in your website. With the Google Photos for WordPress Plugin it's easy to embed your Google Photo Albums using the simple shortcodes.

== Description ==

Display your Google Photo/Picasa Web Albums in your WordPress installation simply with Google Photos & Picasa Viewer . 

* Use Shortcodes to display your albums and album image gallery. 
* The album images are displayed using a lightbox. 
* Admin settings to control size of thumbnail images and visibility settings etc
* Just authenicate with your Google Account and you are ready to go!
* Access your Private and Albums and Photos (Pro Version Only)
* Watch Basic <a href="https://www.youtube.com/watch?v=cx-2PcRcbao" target="_blank">Setup Video</a>

** NEW **
* Touch Sensitive lightbox (Pro Version Only)
* (Got more ideas? Tell me!)

> <strong>Upgrade to Google Photos & Picasa Pro</strong><br>
> If you need support or want to remove the 'Powered by' link as well as better layout options upgrade to <a href="http://www.cheshirewebsolutions.com/?utm_source=cws_gpp_config&utm_medium=text-link&utm_content=readme&utm_campaign=cws_gpp_plugin" rel="friend">Google Photos & Picasa Pro today!</a><br>
> GET 25% OFF! &#8211; use discount code WPMEGA25 on checkout

If you have suggestions for a new add-on, feel free to email me at info@cheshirewebsolutions.com.
Want regular updates? 
follow me on Twitter!
https://twitter.com/CheshireWebSol



== Prerequisites ==

1. PHP5
2. cURL running on your web host


== Installation ==

1. Unzip into your `/wp-content/plugins/` directory
2. Activate the plugin through the 'Plugins' menu in WordPress
3. Make your settings, Admin->Settings->Google Picasa
4. Use the 'Display Album' shortcode [cws_gpp_albums] on a page of your choice.
5. To display the album's images place the shortcode, [cws_gpp_images_in_album] on a page
6. Update the shortcode used in step 4 to include the result_page option. [cws_gpp_albums results_page='page-slug-here']


== Frequently Asked Questions ==

= What if I don't want to display private (unlisted) albums? =

Simple select "Public" option from the 'Show which albums' dropdown menu.

= Does this work with Google Photos? =

Yes this plugin works with images and albums stored and created in Google Photos too.

= Can Users Download the Original Image File =

Yes this is an option on the <a href="http://www.cheshirewebsolutions.com/?utm_source=cws_gpp_config&utm_medium=text-link&utm_content=readme&utm_campaign=cws_gpp_plugin" rel="friend">Pro version</a> 

= The Cache Doesn't Seem to be Working =

Log in to you web host and check the cache/ folder is writable by the web server.


== Screenshots ==

1. This is where you enter the authorization code from Google.
2. This is where you click Allow to authorize access to your Google Web Picasa data.
3. This is the default settings page. 
4. This is an eaxmple of the Albums shortcode [cws_gpp_albums].
5. This is an example of the lightbox displaying photo you clicked on.


== Shortcodes ==

* [cws_gpp_albums] Will display your albums.

* [cws_gpp_images_in_album] This is a place holder to display the results of an album that has been clicked on, on a separate page.

* [cws_gpp_images_by_albumid] Will display images in the album specified via the 'id' attribute


== Shortcode Usage ==

* Display Albums Covers in a Carousel
[cws_gpp_albums theme=carousel dots=1 slidestoshow=3 slidestoscroll=1 autoplay=1 arrows=1 results_page=results-carousel show_details=1 show_title=1 num_results=6 hide_albums='Profile Photos,Auto Backup']

* Display Album Covers in a Grid View
[cws_gpp_albums theme=grid results_page=results-grid show_title=1 show_details=1 num_results=6 hide_albums='Auto Backup,Profile Photos']

* Display Album Covers in a List View
[cws_gpp_albums theme=list results_page=results-list show_title=1 show_details=1 thumb_size=185 num_results=3]

* Display Images from Clicked Album Cover in a Carousel View
[cws_gpp_images_in_album theme=carousel show_title=0 thumbsize=150]

* Display Images from Clicked Album Cover in a Grid View
[cws_gpp_images_in_album theme=grid show_title=1 show_details=1]

* Display Images from Clicked Album Cover in a List View
[cws_gpp_images_in_album theme=list show_title=1 show_details=1 num_results=13 thumb_size=250]

* Display Images in a Specific Album, see 'Album Shortcodes' page for shortcodes complete with your Album IDs. Only one album per page.(PRO VERSION ONLY)
[cws_gpp_images_by_albumid id=5218507736478682657 theme=grid show_title=0 show_details=0]




There are 2 main shortcodes:

* [cws_gpp_albums]
* [cws_gpp_images_album]


Each shortcode will work as is by using the default values saved on the plugin settings page.

The defaults can be overridden by placing attribites on the shortcode below are some examples.


*[cws_gpp_albums]*

Attributes descriptions and examples

theme='grid|list|carousel|propbs|propsg'
results_page='album-results|page-slug-here'
show_title='1|0'
show_details='1|0'
thumb_size='150'
num_results='9'
visibility='all|public|private'
hide_albums='Auto Backup|name of album here'

For example
[cws_gpp_albums theme='grid' results_page='results-list' show_title=1 show_details=1 thumb_size='50' num_results='9' visibility='all']



*[cws_gpp_images_in_album]*

theme='grid|list|carousel'
album_title='1|0'
show_title='1|0'
show_details='1|0'
thumb_size='150'
num_results='9'

For example
[cws_gpp_images_in_album theme='grid' album_title=1 show_title=1  show_details=1]


== Credits ==

* Google Picasa Viewer - Ian Kennerley, http://nakunakifi.com 
* Google PHP Client Library (https://developers.google.com/api-client-library/php/)
* Slick Carouel (http://kenwheeler.github.io/slick/)
* Slick Carousel Lightbox (https://github.com/mreq/slick-lightbox)
* Lightbox2 (http://lokeshdhakar.com/projects/lightbox2)
* Masonry (http://desandro.github.io/masonry/)
* Polaroid Stack Grid - http://tympanus.net/codrops/?p=26096
* Photo Booth strip - http://tympanus.net/codrops/2012/08/01/photo-booth-strips-with-lightbox/
* Cache - http://www.jongales.com/
* Justified Image Grid - Miro Mannino

== Changelog ==

= 3.0.9 =
Added 'Getting Started' sub menu page to admin
Fixed call for style_fx to be Pro only

= 3.0.8 =
Fixed bug where if no theme option was provided in certain shortcodes in could result in feed error notice
Added 'theme=grid' option to shortcode examples in Pro page

= 3.0.7 =
Fixed pagination bug on home page

= 3.0.6 =
Fixed grid link bug with permalinks disabled
Fixed download original link bug where image could open in lightbox

= 3.0.5 =
Fixed grid results layout bug

= 3.0.4 =
Various layout improvements
Carousel options added, arrows, infinite, slidestoshow, slidestoscroll, autoplay, autoplayinterval, speed, dots
Image thumbnail settings bug fixed
Album thumbnail settings bug fixed
Various other little bits

= 2.3.7 =
Added speed variable to init_slick.js
Added empty array check for cache files

= 2.3.6 =
Readme.txt updates and description

= 2.3.5 =
Fixed: Warning: Missing argument notice when using theme pro_pbs (PRO ONLY)
Added isFitWidth to Masonry init to allow for centering of grid via CSS

= 2.3.4 =
Added Show Albums [Public, Private, All, Visible] (PRO ONLY)

= 2.3.3 =
Added Justified Image Grid option (PRO ONLY)

= 2.3.2 =
Fixed bug effecting the sidebar appearance

= 2.3.1 =
Tidy up of error warning notices
Tested with WordPress 4.6.1

= 2.3.0 =
Many small bugfixes.
Rewrote XML from Google Feed
Added 50% Off code
Added Top level menu to admin

= 2.2.3 =
Bug fix: Carousel

= 2.2.2 =
Bux fix: Album Images

= 2.1.2 =
Paginaton added to Show Albums Widget
Added default settings when first installed
Bug fix - pagination under certain circumstance
Among other things

= 2.1.0 =
Changes Title and description.

= 2.0.1 =
Added screenshots

= 2.0 =
Complete rewrite. Brought about by Google turning off OAuth1
Now supports OAuth2
ONLY UPGRADE IF PREVIOUS VERSION STOPPED WORKING FOR YOU!
All shortcodes have changed

= 1.3.2 =
Fixed: Lost settings when updated Settings -> Reading


== Upgrade Notice ==
 
= 2.0 =
Version 2.0 introduces some radical changes to the plugin. Please make sure to back up your data just in case anything happens