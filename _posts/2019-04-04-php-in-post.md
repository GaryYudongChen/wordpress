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

$querystr = "SELECT season FROM Crops_Details ";
$results = $wpdb-&gt;get_results($querystr);
$i=0;
while ($i&lt; count($results)){ echo $results[$i]-&gt;season."
";
$i++;
}
[/insert_php]