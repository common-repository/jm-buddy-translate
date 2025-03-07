=== JM Buddy Translate  ===
Contributors: jonathanmoorebcsorg
Donate link: http://paypal.me/jonathanmoorebcsorg
Tags: locale, language, translate, back-end, front-end, buddypress, bbPress
Requires at least: 4.7
Tested up to: 4.8.3
Stable tag: trunk
License: GPLv3
License URI: https://www.gnu.org/licenses/gpl.txt

Quick and easy translate BuddyPress and bbPress messages or any selected text.
[![Build Status](https://travis-ci.org/Jon007/jm-buddy-translate.svg?branch=master)](https://travis-ci.org/Jon007/jm-buddy-translate)
[![project status](http://www.repostatus.org/badges/latest/active.svg)](https://github.com/Jon007/jm-buddy-translate)
[![GitHub GitHub latest](https://img.shields.io/github/release/Jon007/jm-buddy-translate.svg)](https://github.com/Jon007/jm-buddy-translate/releases)
[![Wordpress  Wordpress latest](http://img.shields.io/wordpress/plugin/v/jm-buddy-translate.svg)](https://wordpress.org/plugins/jm-buddy-translate)
[![Wordpress downloads](http://img.shields.io/wordpress/plugin/dt/jm-buddy-translate.svg)](https://wordpress.org/plugins/jm-buddy-translate/)
[![Wordpress rating](http://img.shields.io/wordpress/plugin/r/jm-buddy-translate.svg)](https://wordpress.org/plugins/jm-buddy-translate/)
[![license](https://img.shields.io/github/license/Jon007/jm-buddy-translate.svg)](https://github.com/Jon007/jm-buddy-translate/blob/master/LICENSE)

== Description ==

Adds Translate button to the WordPress admin bar to translate any selected text.
Adds Translate buttons to BuddyPress and bbPress messages.

Translate translates selected text to current locale: where user is logged in, this is the user's preferred language.

Perfect for a multilingual Buddypress site, this tool allows your users to translate messages to their own language.

Other tools translate the whole site but a polyglots and language learners may not want this, for learning it is best to see the original, and translate only where necessary.
Or the whole site may be already translated to your preferred language but you are getting messages from other users (or from some untranslated plugin) and you want to translate those.

Currently uses Google Translate.

== Installation ==

This section describes how to install the plugin and get it working.

1. Upload the plugin files to the `/wp-content/plugins/plugin-name` directory, or install the plugin through the WordPress plugins screen directly.
1. Activate the plugin through the 'Plugins' screen in WordPress
1. Use the Settings->Plugin Name screen to configure the plugin
(By default the Translate buttons are turned on in all applicable contexts, in Settings you can individually turn off contexts and you can see a few hints on usage.)


== Frequently Asked Questions ==

= How do I change the style of the translation results? =

Each element in the popup translation window has a separate id so it can be restyled easily.

= What browsers has this been tested with? =

This tool has been tested ok with up to date versions of Chrome, Firefox, Safari and Opera Browsers on desktop and mobile.
It's also been tested Microsoft Internet Explorer and Edge with the following notes:
It’s preferable to use Chrome, Firefox, Safari, Opera etc to avoid problems with Microsoft browsers.

= Why do I get a warning from Internet Explorer? =

When the translation tool requests data from Google Translate, Internet Explorer may do an extra check to confirm that the certificate for googleapis.com has not been revoked.
In certain circumstances (for example if the user is located in China and does not have VPN enabled), Internet Explorer may unable to complete this check so will give the warning.
It is possible to accept and continue or to turn off certificate revocation check.
Once accepted the tool 

= Why can't I translate with Microsoft Edge? =

See above point for Internet Explorer:  the same applies, though Edge browser may be even more strict and fail without giving appropriate error message or opportunity to continue.

Note that whatever the problem, the translation result panel link to Google Translate is still available and will open Google Translate with the selected text.


== Screenshots ==

1. Illustration shows sample usage along with recommended tool jsm-user-locale which provides current user a quick way to choose preferred language. When you click the translate button, the currently text is sent to Google translate for translation to current user language.

2. BuddyPress and bbPress usage: The tool includes hooks to insert translate buttons along in the standard button areas for bbPress and BuddyPress messages and activities.

3. In the settings screen you can turn on or off the various integrations.

== Changelog ==

= 1.0.9 =
* formatting improvements for bbPress
* stub code for auto-translate posts (uncomment call at end of .js file to enable)

= 1.0.8 =
* updates to documentation and packaging

= 1.0.7 = 
(2017/04/08) Minor fixes:
* updated Settings screen to use WP settings api
* fixes for change to google results format
* improved default message and readability styling
* Languages: updated Spanish, Chinese, added French

= 1.0.2 = 
(2017/04/06) Minor fixes:
* Change to load sequence for admin views due to some "headers already sent" type issues.
* removed https from google translate link to allow use in non-SSL site

= 1.0.1 =
(2017/04/05) Patching for Internet Explorer compatibility.

= 1.0 =
(2017/04/04) Initial release.


== Upgrade Notice ==

= 1.0.7 =
First version published on wordpress.org repository, readme etc updated to comply with latest guidelines.


= Repositories =

* [GitHub](https://github.com/Jon007jm-buddy-translate/)
* [WordPress.org](https://plugins.svn.wordpress.org/jm-buddy-translate/)

= Recommended Plugins: =

This tool does not require any other plugins, however is tested with and recommended for use with:
* [BuddyPress](https://wordpress.org/plugins/buddypress/) Version 2.8.2
* [bbPress](https://wordpress.org/plugins/bbpress/) Version 2.5.12
The tool is intended to add translate links for messages and docs with these tools.
For other inputs, the Admin Bar translate button still allows translation of selected text.

The following tool is also very useful for quickly changing current user language:
* [JSM's User Locale](https://wordpress.org/plugins/jsm-user-locale/) 1.2.2
The translation tool uses User Locale as the target language: if you enable JSM’s User Locale, you can quickly change the front-end language, which also becomes the target language for translations.


== Contribution ==

If you have a feature request, or if you have developed the feature already, please feel free to use the [Issues](https://github.com/Jon007/jm-buddy-translate/issues) and/or (Pull Requests)[https://github.com/Jon007/jm-buddy-translate/pulls] section.

Plugin translations are provided for English, French, Spanish, Chinese, please feel to contribute more [translations](https://translate.wordpress.org/projects/wp-plugins/jm-buddy-translate).
