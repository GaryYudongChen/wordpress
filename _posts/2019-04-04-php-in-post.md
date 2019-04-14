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

$querystr = "SELECT Crop_Type FROM CropType";  
$results = $wpdb->get_results($querystr);  
$i=0;  
while ($i< count($results)){  
echo $results[$i]->Crop_Type."<br />";  
$i++;  
} 
[/insert_php]