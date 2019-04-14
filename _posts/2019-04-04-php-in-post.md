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
$helloworld_id = $wpdb->get_var("SELECT ID FROM wp_posts WHERE post_name = 'u5-map'");
echo $helloworld_id;
$querystr = "SELECT ID FROM test_table";  
$results = $wpdb->get_results($querystr);  
$i=0;  
while ($i< count($results)){  
echo $results[$i]->ID."<br />";  
$i++;  
} 
[/insert_php]