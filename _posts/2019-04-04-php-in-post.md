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
define(‘PATH’, dirname(dirname(__FILE__)).‘/’);  
require_once(PATH . ‘../wp-blog-header.php’);  
global $wpdb;
$querystr = "SELECT ID FROM wordpress.wp_posts";  
$results = $wpdb->get_results($querystr);  
$i=0;  
while ($i< count($results)){  
echo $results[$i]->column_1."<br />";  
$i++;  
}  
[/insert_php]