=== Quick Configuration Links ===
Contributors: whiteshadow
Donate link: http://w-shadow.com/
Tags: configuration, admin, plugins, settings, usability, menu
Requires at least: 2.5
Tested up to: 5.7
Stable tag: 1.4.9

Automagically adds a "Settings" link to every active plugin on the "Plugins" page.

== Description ==

This plugin will add a "Settings" link to every active plugin listed on the "Plugins" page (right next to the "Deactivate" and "Edit" links). This makes it easy to acccess plugin configuration without hunting through the entire dashboard menu. 

The plugin finds the right admin page by automatically scanning through the WordPress menu structure to detect configuration-related plugin pages. Lab trials shown success rate of over 95%.

Additional notes : 

* *Quick Configuration Links* will automatically skip plugins that add their own custom link(s) to their "Plugins" page listing.
* If a plugin has only one menu entry, the "Settings" link will always point to that page - even it has nothing to do with configuration. This is by design.

== Installation ==

Install it just like any other plugin : 

1. Download the .zip archive and extract it.
2. Upload the `quick-configuration-links` directory to the `/wp-content/plugins/` directory
3. Activate the plugin through the 'Plugins' menu in WordPress

You may need to refresh the page before the "Settings" will appear.

== Changelog ==

= 1.4.9 =
* Fixed a potential fatal error that could be caused by an uncaught exception.
* Tested up to WordPress 5.2.

= 1.4.8 =
* Fixed the "array_shift() expects parameter 1 to be array, object given" warning that showed up when using the plugin with WP 4.7.

= 1.4.6 =
* Tested up to WordPress 4.2.

= 1.4.5 =
* Tested up to WP 4.2-alpha.
* Fixed a URL generation bug that caused the plugin to display non-functioning "Settings" links for plugins that place their settings page under a custom top level menu (e.g. "My Plugin -> Settings").
