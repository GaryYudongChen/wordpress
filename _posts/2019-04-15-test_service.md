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
[insert_php]

[test]

echo 'next';

global $wpdb;
$querystr = "SELECT term_id FROM wp_terms";  
$results = $wpdb->get_results($querystr);  
$i=0;  
while ($i< count($results)){  
echo $results[$i]->term_id."<br />";  
$i++;  
}  

[/insert_php]