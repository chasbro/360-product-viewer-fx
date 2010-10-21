=== 360 Product Viewer FX ===
Contributors: flashxml
Tags: images, photos, widget, post, plugin, posts, sidebar, free, flash, 360, product, viewer, xml, text, as3, effects, reflection, skin, images, auto, rotate, autoplay
Requires at least: 2.8.0
Tested up to: 3.0.1
Stable tag: trunk

An advanced 360 Product Viewer. Fully XML customizable without any Flash knowledge. And it's free!

== Description ==

You can integrate it in any website for free without even using Flash. The rotation speed is customizable and can be set to autoplay. The controls (navigation, zoom in/out, play/pause) have customizable skins. It has the possibility to use HTML/CSS formated text and there are different properties for reflection. There are other customizable properties on the Live Demo.

== Installation ==

Make sure your Wordpress version is greater than 2.8 and your hosting provider is using PHP5.

1. There are two files to download: [WordPress Plugin](http://downloads.wordpress.org/plugin/360-product-viewer-fx.zip "360 Product Viewer FX Plugin") (that you have to install and activate) & [Free archive](http://www.flashxml.net/free/download/360-product-viewer.zip "360 Product Viewer FX")
2. Create a new folder inside your **wp-content** folder called **flashxml**, inside this folder create a new one called **360-product-viewer-fx** and copy the content of the **free archive** there
3. If you copied the **free archive** to a location different than the one above, go to **360 Product Viewer FX** from the **Settings** tab in your **WordPress Dashboard** and update the path accordingly
4. Add `[360-product-viewer-fx][/360-product-viewer-fx]` where you want the Flash to show up in your post/page
5. If you want to make the 360 Product Viewer FX part of your theme, edit the template files and add `<?php productviewerfx_echo_embed_code(); ?>` where you want it to show up
6. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your 360 Product Viewer FX](http://www.flashxml.net/360-product-viewer.html "360 Product Viewer FX") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `wp-content/flashxml/360-product-viewer-fx/settings.xml`
7. To use your own images, upload them to `wp-content/flashxml/360-product-viewer-fx/images/` and update the `wp-content/flashxml/360-product-viewer-fx/images.xml` file accordingly

= Additional settings file =

To embed the 360 Product Viewer FX more than once, you will need another settings file and (probably) another set of images. Let's assume your new file is called `settings2.xml`. Add `[360-product-viewer-fx settings="settings2.xml"][/360-product-viewer-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the file name as **the first argument** of the `productviewerfx_echo_embed_code()` function call (for example `<?php productviewerfx_echo_embed_code("settings2.xml"); ?>`).

= No Flash support text =

To support visitors without Adobe Flash Player, you can provide alternative content by adding the text between `[360-product-viewer-fx]` and `[/360-product-viewer-fx]`. If you made the Flash part of your theme, add the text as **the second argument** of the `productviewerfx_echo_embed_code()` function call (for example `<?php productviewerfx_echo_embed_code("","Alternative content"); ?>`).

= If you have PHP4 =

To make it work with PHP4, add `[360-product-viewer-fx width="600" height="300"][/360-product-viewer-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the width and height as **the third and fourth argument** of the `productviewerfx_echo_embed_code()` function call. Don't forget to provide your own width and height values, since 600 and 300 are just examples.

= Getting rid of the FlashXML.net label =

To remove the FlashXML.net label from the top-left corner you'll need to buy the [paid package](http://www.flashxml.net/360-product-viewer.html "360 Product Viewer FX"). Once you'll do that, simply use the SWF file from the paid package to overwrite the SWF file from the `wp-content/flashxml/360-product-viewer-fx/` folder.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/360-product-viewer.html "360 Product Viewer FX") is the utility that helps easily customize your 360 Product Viewer FX to fit all your needs.