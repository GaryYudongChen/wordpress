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
require_once(ABSPATH . 'wp-config.php');
$connection = mysql_connect($DB_HOST, $DB_USER, $DB_PASSWORD);
mysql_select_db($DB_NAME);

$user_count = $wpdb-get_var( "SELECT COUNT(*) FROM $wpdb-users" );   
[/insert_php]