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
   global $wpdb;
   $mylink = $wpdb -> get_var( "SELECT ID FROM $wpdb_users WHERE user_login = 'admin'" );
   echo $mylink;
   echo "fuck";
[/insert_php]