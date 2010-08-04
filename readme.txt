=== 360 Product Viewer FX ===
Contributors: flashxml
Tags: images, photos, widget, post, plugin, posts, sidebar, free, flash, 360, product, viewer, xml, text, as3, effects, reflection, skin, images, auto, rotate, autoplay
Requires at least: 2.8.0
Tested up to: 3.0
Stable tag: trunk

== Description ==

An advanced 360 product viewer. Fully XML customizable, without using Flash. And it's free!

= Main features =

You can integrate it in any website for free without even using Flash. The rotation speed is customizable and can be set to autoplay. The controls (navigation, zoom in/out, play/pause) have customizable skins. It has the possibility to use HTML/CSS formated text and there are different properties for reflection. There are other customizable properties on the Live Demo.

== Installation ==

Make sure your Wordpress version is greater than 2.8 and your hosting provider is using PHP5.

1. [Download](http://www.flashxml.net/free/download/360-product-viewer.zip "360 Product Viewer FX") or [purchase](http://www.flashxml.net/360-product-viewer.html#swmi-license "360 Product Viewer FX") the 360 Product Viewer FX Flash component
2. Create a new folder inside your `/wp-content/` directory called `flashxml/360-product-viewer-fx` and copy the content of the archive to this folder
3. Install [the plugin](http://downloads.wordpress.org/plugin/360-product-viewer-fx.zip "360 Product Viewer FX Plugin") or upload the `360-product-viewer-fx` folder along with all its files to `/wp-content/plugins/` directory
4. Activate the plugin from the **Plugins** tab in **WordPress Dashboard**
5. Go to **360 Product Viewer FX** from the **Settings** tab and update the path in case you used a different one
6. In the post editor use the following tag to embed the 360 Product Viewer FX: `[360-product-viewer-fx][/360-product-viewer-fx]`. You could also add `<?php productviewerfx_echo_embed_code(); ?>` in the PHP file of your theme
7. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your 360 Product Viewer FX](http://www.flashxml.net/360-product-viewer.html "360 Product Viewer FX") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `flashxml/360-product-viewer-fx/settings.xml`
8. To use your own images, upload them to the `flashxml/360-product-viewer-fx/images` folder and update the `flashxml/360-product-viewer-fx/images.xml` file accordingly

= Additional settings file =

To embed the 360 Product Viewer FX more than once, you will need another settings file and (probably) another set of images. Let's assume your new file is called **settings2.xml**. From the post editor, use the following code: `[360-product-viewer-fx settings="settings2.xml"][/360-product-viewer-fx]`. From the PHP files of your theme, add the file name as *the first argument* of the `productviewerfx_echo_embed_code()` function call. If you use a separate set of images, don't forget to create a new XML file for that and update the value in the settings file.

= No Flash support text =

To support visitors without Adobe Flash, you can provide alternative textual content. From the post editor, add the text between `[360-product-viewer-fx]` and `[/360-product-viewer-fx]`. From the PHP files of your theme, add the text as *the second argument* of the `productviewerfx_echo_embed_code()` function call.

= If you have PHP4 =

To make it work if you're using PHP4, add the following code `[360-product-viewer-fx width="600" height="300"][/360-product-viewer-fx]` in the post editor. From the PHP files of your theme, add the width and height as *the third and fourth argument* of the `productviewerfx_echo_embed_code()` function call. Don't forget to provide your own width and height values, since 600 and 300 are just examples.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/360-product-viewer.html "360 Product Viewer FX") is the utility that helps easily customize your 360 Product Viewer FX to fit all your needs.