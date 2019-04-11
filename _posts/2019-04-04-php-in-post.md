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
echo 'time is';
require_once(ABSPATH . 'wp-config.php');
$connection = mysqli_connect(DB_HOST, DB_USER, DB_PASSWORD);
mysqli_select_db($connection, DB_NAME);

$results = $wpdb->get_results( "SELECT * FROM $table_name"); 
if(!empty($results)) 
{
   echo "<table width='100%' border='0'>"; 
   echo "<tbody>";      
   echo "$results";
[/insert_php]