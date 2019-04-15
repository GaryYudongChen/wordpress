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
$querystr = "SELECT column_1 FROM test_table";  
$results = $wpdb->get_results($querystr);  
$i=0;  
while ($i< count($results)){  
echo $results[$i]->column_1."<br />";  
$i++;  
}  

[/insert_php]