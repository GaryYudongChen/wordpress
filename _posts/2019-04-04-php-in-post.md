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

$querystr = "SELECT poste_title FROM wp_posts";
$results = $wpdb->get_results($querystr);
$i=0;
while ($i< count($results))
{ 
   echo $results[$i]->poste_title."<br />";
   $i++;
}
[/insert_php]