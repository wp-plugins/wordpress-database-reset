=== WordPress Database Reset ===

Contributors: mousesports
Tags: wordpress, database, database-reset, default-settings, default, wp-reset, security, secure
License: GPL2
Requires at least: 3.0
Tested up to: 3.2.1
Stable tag: 1.2

A secure and easy way to reinitialize the WordPress database to its default settings.

== Description ==

WordPress Database Reset is a secure and easy way to reinitialize your WordPress database back to its default settings without actually having to reinstall WordPress yourself.

Theme and plugin developers tend to forget to clean up after themselves and lots of junk gets piled into the WordPress database (most likely the wp_options table).

This plugin allows you to securely reset the database, deleting everything except the admin user. The plugin makes sure the only access it will grant is to administrators with a user level of 10. Also, the form uses nonces (read more about them at <a href="http://codex.wordpress.org/WordPress_Nonces">WordPress nonces</a>) which adds another level of security to your application.

== Installation ==

Copy the wp-reset folder and its contents to your wp-content/plugins directory,
then activate the plugin. You could also use the built-in Add New Plugin
feature within WordPress. After activating, you will automatically be redirected
to the plugin page.

== Frequently Asked Questions ==

= Why reset the database? =

There are two important reasons as to why I built this plugin:

1. I wanted a simple and painless way to obtain a fresh clean database without actually having to reinstall WordPress.
2. 9 times out of 10 I get tons of excess junk in the wp_options table after installing plugins and themes that do not clean up after themselves.

== Screenshots ==
1. The plugin page - a more secure way of resetting your database.

== Changelog ==
= 1.2 =
* Added capability to manually select whether or not plugin should be reactivated upon reset
* Modified class name to avoid potential conflicts with WordPress core
* Modified wp_mail override
* Removed deprecated user level for WordPress 3.0+
* Fixed small bug where if admin user did not have admin capabilities, it would tell the user they did

= 1.0 =
* First version