=== 3D Banner ===
Contributors: johnsmith48
Tags: flash, 3d, banner, images, video, free, widget, css, effects, animation, text, html
Requires at least: 2.8.0
Tested up to: 3.1
Stable tag: trunk

Probably the best 3D Banner on the web. Fully XML customizable, without any Flash knowledge. And it's free!

== Description ==

You can integrate it in any website for free without any Flash knowledge. Customizable width and height of the overall banner, up to 1680 x 1050 pixels. It has awesome 3D image transitions with lots of shade and background properties. The text is HTML/CSS formatted. The navigation buttons can be placed o various positions and are skinnable. A lot of other properties in the Live Demo.

== Installation ==

Make sure your Wordpress version is greater than 2.8 and your hosting provider is using PHP5.

1. There are two files to download: [WordPress Plugin](http://downloads.wordpress.org/plugin/3d-banner-fx.zip "3D Banner FX Plugin") (that you have to install and activate) & [Free package](http://www.flashxml.net/free/download/3d-banner.zip "3D Banner FX")
2. Create a new folder inside your **wp-content** folder called **flashxml**, inside this folder create a new one called **3d-banner-fx** and copy the content of the **free package** there
3. If you copied the **free package** to a location different than the one above, go to **3D Banner FX** from the **Settings** tab in your **WordPress Dashboard** and update the path accordingly
4. Add `[3d-banner-fx][/3d-banner-fx]` where you want the Flash to show up in your post/page
5. If you want to make the 3D Banner FX part of your theme, edit the template files and add `<?php 3dbannerfx_echo_embed_code(); ?>` where you want it to show up
6. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your 3D Banner FX](http://www.flashxml.net/3d-banner.html "3D Banner FX") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `wp-content/flashxml/3d-banner-fx/settings.xml`
7. To use your own images, upload them to `wp-content/flashxml/3d-banner-fx/images` and update the `wp-content/flashxml/3d-banner-fx/images.xml` file accordingly

= Additional settings file =

To embed the 3D Banner FX more than once, you will need another settings file and (probably) another set of images. Let's assume your new file is called `settings2.xml`. Add `[3d-banner-fx settings="settings2.xml"][/3d-banner-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the file name as **the first argument** of the `3dbannerfx_echo_embed_code()` function call (for example `<?php 3dbannerfx_echo_embed_code("settings2.xml"); ?>`).

= Add as widget =
To add the 3D Banner FX as a widget, go to **Widgets** from the **Appearance** tab in your *WordPress Dashboard*, then drag and drop the 3D Banner FX from **Available Widgets** to the widget area you want. You can specify a different `settings.xml` file and an alternative content for users without Adobe Flash Player from the widget's settings.

= No Flash support text =

To support visitors without Adobe Flash Player, you can provide alternative content by adding the text between `[3d-banner-fx]` and `[/3d-banner-fx]`. If you made the Flash part of your theme, add the text as **the second argument** of the `3dbannerfx_echo_embed_code()` function call (for example `<?php 3dbannerfx_echo_embed_code("","Alternative content"); ?>`).

= If you have PHP4 =

To make it work with PHP4, add `[3d-banner-fx width="600" height="300"][/3d-banner-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the width and height as **the third and fourth argument** of the `3dbannerfx_echo_embed_code()` function call. Don't forget to provide your own width and height values, since 600 and 300 are just examples.

= Getting rid of the FlashXML.net label =

To remove the FlashXML.net label from the top-left corner you'll need to buy the [paid package](http://www.flashxml.net/3d-banner.html "3D Banner FX"). Once you'll do that, simply use the SWF file from the paid package to overwrite the SWF file from the `wp-content/flashxml/3d-banner-fx/` folder.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/3d-banner.html "3D Banner FX") is the utility that helps easily customize your 3D Banner FX to fit all your needs.