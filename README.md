# wordpress-plugins
Useful plugins for Wordpress that I use in development

## SEO & Permalinks

- [WP Translitera](https://wordpress.org/plugins/wp-translitera/) - Plug-in for transliteration permanents links of records, pages, tag, media and files.
> I use it because the previous popular plugin ([Cyr to Lat enhanced](https://wordpress.org/plugins/cyr3lat/)) did not receive an update for more than 4 years.

- [Yoast SEO](https://wordpress.org/plugins/wordpress-seo/) - With Yoast SEO, you get a solid toolset that helps you aim for that number one spot in the search results. Yoast: SEO for everyone.

- [All in One SEO Pack](https://wordpress.org/plugins/all-in-one-seo-pack/) - Use All in One SEO Pack to optimize your WordPress site for SEO. It’s easy and works out of the box for beginners, and has advanced features and an API for developers.

- [Google XML Sitemaps](https://wordpress.org/plugins/google-sitemap-generator/) - Automatically generate an XML sitemap.

- [Broken Link Checker](https://wordpress.org/plugins/broken-link-checker/) - This plugin will monitor your blog looking for broken links and let you know if any are found.


## Development

- [Theme Check](https://wordpress.org/plugins/theme-check/) - Test your theme and make sure it’s up to spec with the latest theme review standards.

- [Query Monitor](https://wordpress.org/plugins/query-monitor/) - Query Monitor is the developer tools panel for WordPress. It enables debugging of database queries, PHP errors, hooks and actions, block editor blocks, enqueued scripts and stylesheets, HTTP API calls, and more.

- [User Role Editor](https://wordpress.org/plugins/user-role-editor/) - Easy change user roles and capabilities.

- [FakerPress](https://wordpress.org/plugins/fakerpress/) - Generate dummy data.


## Custom Post Types, Taxonomies, Meta fields, UI

- [Custom Post Type UI](https://wordpress.org/plugins/custom-post-type-ui/) -  Helps in creating additional custom post types, taxonomies.

- [Advanced Custom Fields Pro](https://www.advancedcustomfields.com/pro/) :moneybag: - Custom fields, meta boxes, theme optionsm sliders, maps, galleries etc. [Free version](https://wordpress.org/plugins/advanced-custom-fields/)


## Multilingual  Internalization

- [Polylang](https://wordpress.org/plugins/polylang/) - Polylang allows you to create a bilingual or multilingual WordPress site. 

- [WPML](https://wpml.org) :moneybag: - WPML makes it easy to build multilingual sites and run them. It’s powerful enough for corporate sites, yet simple for blogs. 

- [Loco Translate](https://wordpress.org/plugins/loco-translate/) - Loco Translate provides in-browser editing of WordPress translation files. 


## Post Editing, Content, Order

- [Duplicate Post](https://wordpress.org/plugins/duplicate-post/) - This plugin allows users to clone posts of any type, or copy them to new drafts for further editing. 

- [Post Types Order](https://wordpress.org/plugins/post-types-order/) - A powerful plugin, Order Posts and Post Types Objects using a Drag and Drop Sortable JavaScript capability. 


## Images

- [WebP Express](https://ru.wordpress.org/plugins/webp-express/) - Plugin generates WebP images and improves img tag. (Good for mobile users)

- [Regenerate Thumbnails](https://wordpress.org/plugins/regenerate-thumbnails/) - Regenerate Thumbnails allows you to regenerate all thumbnail sizes for one or more images that have been uploaded to your Media Library.

- [Compress JPEG & PNG images](https://wordpress.org/plugins/tiny-compress-images/) - This plugin automatically optimizes all your images by integrating with the popular image compression services TinyJPG and TinyPNG.


## Backup, Transfer

- [Duplicator](https://wordpress.org/plugins/duplicator/) - Standard WordPress migration and WordPress backups are easily handled by this plugin 


## Firewall, Defense, Security

- [WordFence](https://wordpress.org/plugins/wordfence/) - Wordfence includes an endpoint firewall and malware scanner that were built from the ground up to protect WordPress. 

- [All In One WP Security & Firewall](https://ru.wordpress.org/plugins/all-in-one-wp-security-and-firewall/) - Security & Firewall plugin


## Login, Registration, Social Sharing

- [Super Socializer](https://wordpress.org/plugins/super-socializer/) - Integrate Social Login, Social Share and Social Comments at your website easiest and simplest possible way.


## Dashboard

- [Adminimize](https://ru.wordpress.org/plugins/adminimize/) - Clean up the WordPress admin area, for example activate/deactivate every part of the menu and the sub-menu etc.

- [File Manager](https://wordpress.org/plugins/wp-file-manager/) - File manager allows you to edit, delete, upload, download, zip, copy and paste files and folders directly from the wordpress backend. 


## Cache

- [WP Super Cache](https://ru.wordpress.org/plugins/wp-super-cache/) - Static caching plugin.

- [W3 Total Cache](https://ru.wordpress.org/plugins/w3-total-cache/) - Another caching plugin.


## eCommerce | WooCommerce

- [WooCommerce](https://wordpress.org/plugins/woocommerce/) - Shop plugin.

- [YITH WooCommerce Wishlist](https://wordpress.org/plugins/yith-woocommerce-wishlist/) - Extension for creating Wishlists.

- [YITH WooCommerce Compare](https://wordpress.org/plugins/yith-woocommerce-compare/) - Extension that allow your users to compare some products of your shop.

- [WooCommerce Autocomplete search bar](https://wordpress.org/plugins/woo-autocomplete-search-bar/) - Autocomplete search bar allows your users to search through all WooCommerce products, categories, tags, or taxonomy.

## Miscellaneous (Misc)

### Debug
For debugging it's a good thing to turn on the "debug" mode. 
Also with debug logs and show errors and warnings as they are generated:
In wp-config.php:
```php
define( 'WP_DEBUG', true );
define( 'WP_DEBUG_LOG', true );
define( 'WP_DEBUG_DISPLAY', false );
```

### Revisions
You can set the number of revisions in wp-config.php by adding:
```php
define( 'WP_POST_REVISIONS', 3);
```
Where 3 - is the number of revisions. If set to false - no further revisions will be generated, if true - turn-on revision creation.
Also you can change the time interval for revision creation.
```php
define( 'AUTOSAVE_INTERVAL', 600 );
```

To remove all revisions from DB hard way - you can run query:
```sql
DELETE from wp_posts WHERE post_type = “revision”;
```