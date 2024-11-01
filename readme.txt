=== Visual Admin Customizer ===
Contributors: whiteshadow
Tags: admin, customization, branding, hide
Requires at least: 4.6
Tested up to: 5.7
Stable tag: 1.0.4

Hide almost any part of the WordPress admin by using a visual editor.

== Description ==
Hide almost any part of the WordPress admin area by using a visual, point-and-click editor. You can hide things from all users or only from specific roles. You can also add your own CSS to the WordPress admin (per role).

This plugin does not have a fixed list of things it can customize. Instead, it displays a live version of the WordPress dashboard and lets you select the parts of the page that you want to hide. You can hide almost any unique element (but see the "Limitations" section below).

Here are a few examples of things you can hide:
* Dashboard widgets.
* Post editor meta boxes.
* Custom fields.
* Screen options.
* Individual buttons.
* Text boxes, checkboxes, dropdown lists and most other form fields.

= Requirements =
* PHP 5.3 and up.
* A modern browser like Firefox, Chrome or IE 9 and up. 

= Limitations =
* This is not a security tool. The changes it makes are cosmetic. Users who are familiar with web development can bypass them. Don't use it for security-critical tasks.
* It's not great at hiding dynamic content like dialog windows, pop-up menus, or any content that changes frequently or depending on the logged-in user.
* It's intended for customizing *unique* things like specific meta boxes or buttons. If you want to do something like hide *all* "Edit" links on a page or change the appearance of *all* "Save Changes" buttons, you'll have to write the CSS code yourself or use a different plugin.

== Installation ==
1. Install the plugin through the WordPress "Plugins" screen, or upload the plugin files to the `/wp-content/plugins/visual-admin-customizer` directory.
2. Activate the plugin through the "Plugins" screen.
3. To start customizing the admin panel, go to "Tools -> Admin Customizer".

== Screenshots ==

1. Plugin configuration screen
2. Add custom CSS to the WordPress admin

== Changelog ==

= 1.0.4 =
* Added a potential workaround for a JS error about (...).split not being a function.
* Fixed a severe performance bug that could cause high JS memory usage and browser freezing when trying to hide things on pages where the body tag has too many classes.
* Tested up to WordPress 5.5.

= 1.0.3 =
* Fixed a PHP 5.3 compatibility issue.
* Tested up to WordPress 5.2.

= 1.0.2 =
* Fixed a potential conflict that could cause PHP errors like this: "An exception occurred: Call to undefined method Ajaw_v1_ActionBuilder::permissionCallback()".

= 1.0.1 =
* Fixed a bug where the "Changes" table could overflow the pop-up panel when the selector got too long.
* Fixed a fatal error on admin pages that don't have a valid WP_Screen instance (e.g. various pop-ups).
* Fixed several minor bugs related to admin notices.
* Tested up to WordPress 4.9.

= 1.0 =
* Initial release.