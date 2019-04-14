---
ID: 194
post_title: PHP in post
author: admin
post_excerpt: ""
layout: post
permalink: http://www.lumus.ga/php-in-post/
published: true
post_date: 2019-04-04 03:15:34
---
[insert_php]
echo 'time is';
[/insert_php]
[insert_php]
 
global $wpdb;
$helloworld_id = $wpdb->get_var("SELECT ID FROM wp_posts WHERE post_name = 'u5-map'");
echo $helloworld_id;
[/insert_php]