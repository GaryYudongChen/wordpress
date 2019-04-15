---
ID: 460
post_title: test_service
author: admin
post_excerpt: ""
layout: post
permalink: http://www.lumus.ga/test_service/
published: true
post_date: 2019-04-15 01:33:57
---
echo [wbcr_snippet id="458"];
[insert_php]
global $wpdb;
$querystr= "SELECT name FROM wp_terms`";  
$result= $wpdb->get_results($querystr);  
$i=0;  
while ($i< count($querystr)){  
echo $data[$i]->name."<br />";  
$i++;  
} 
[/insert_php]