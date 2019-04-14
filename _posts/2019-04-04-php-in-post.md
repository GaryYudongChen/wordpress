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
$querystr = "SELECT ID FROM wordpress.wp_posts";  
$results = $wpdb->get_results($querystr);  
$i=0;  
while ($i< count($results)){  
echo $results[$i]->column_1."<br />";  
$i++;  
}    
[/insert_php]