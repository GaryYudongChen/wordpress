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

$querystr = "SELECT post_name FROM wp_posts";  
$results = $wpdb->get_results($querystr);  
$i=0;  
while ($i< count($querystr)){  
echo $results[$i]->post_name."<br />";  
$i++;  
} 
[/insert_php]