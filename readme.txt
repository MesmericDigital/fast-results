=== Fast Results ===
Author URI: https://github.com/OllieJones
Plugin URI: https://plumislandmedia.net/wordpress-plugins/fast-results/
Donate link: 
Contributors:  Ollie Jones
Tags: cache, performance, pagination
Requires at least: 5.9
Tested up to: 6.4
Requires PHP: 5.6
Stable tag: 0.1.3
License: GPLv2
Github Plugin URI: https://github.com/OllieJones/fast-results
License URI: https://www.gnu.org/licenses/gpl-2.0.html

Generates results pages (product pages, archive pages) fast for large sites.

== Description ==

It takes time to generate results pages, especially the pagination UI, on large sites and stores. This plugin makes that operation faster.

It requires a [persistent object cache](https://developer.wordpress.org/reference/classes/wp_object_cache/#persistent-cache-plugins) to do anything useful.

Thanks to Jetbrains for the use of their software development tools, especially [PhpStorm](https://www.jetbrains.com/phpstorm/). It's hard to imagine how a plugin like this one could be developed without PhpStorm's tools for exploring epic code bases like WordPress's.

== Performance and Reliability Tips ==

1. **Use a Persistent Object Cache**: Ensure that you have a persistent object cache plugin installed and configured. This plugin relies on it for optimal performance.
2. **Optimize Database Queries**: Regularly check and optimize your database queries. Avoid using `SQL_CALC_FOUND_ROWS` for large datasets as it can be inefficient.
3. **Monitor Performance**: Use tools like Query Monitor to keep an eye on your site's performance and identify any bottlenecks.
4. **Regular Updates**: Keep your WordPress, themes, and plugins updated to the latest versions to benefit from performance improvements and security patches.
5. **Error Handling**: Implement proper error handling for database queries to ensure reliability.
6. **Logging**: Enable logging for performance metrics to help identify and troubleshoot issues.

== Frequently Asked Questions ==

= How can this plugin keep accurate track of which archive page navigation sequence is in use? =

It uses the same techniques used in WordPress core for the [WP_Query cache](https://github.com/WordPress/wordpress-develop/blob/6.3/src/wp-includes/class-wp-query.php#L3173).


== Installation ==

1. Go to `Plugins` in the Admin menu
2. Click on the button `Add new`
3. Click on Upload Plugin
4. Find `fast-results.zip` and upload it
4. Click on `Activate plugin`


== Changelog ==

= 0.1.3 October 30, 2023
Optimized SQL queries, added error handling and logging, and updated documentation.

= 0.1.2 October 30, 2023
Cleanup.

= 0.1.1 October 13, 2023
Birthday of Fast Results.
