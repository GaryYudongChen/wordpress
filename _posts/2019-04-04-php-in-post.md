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
$host = "localhost:3306";
$username = "root";
$password = "FIT5120lumus";
$dbname = "test";
$connection = mysql_connect($host, $username, $password, $dbname);

   $sql = "select * from croptype;";
   $result = mysqli_query($connection, $sql);
   $resultCheck = mysqli_num_rows($result);
   
   if ($resultCheck >0)
   {
      while ($row = mysqli_fetch_assoc($result))
	  {
	     echo $row['Crop_Type'];
	  }
   }
[/insert_php]