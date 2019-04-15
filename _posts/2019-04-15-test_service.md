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
$data = "SELECT name FROM wp_terms`";  
$show = $wpdb->get_results($data);  
$i=0;  
while ($i< count($data)){  
echo $data[$i]->name."<br />";  
$i++;  
} 
[\insert_php]