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
echo 'Server date and time is: ';
echo date('l, F j, Y \a\t G:i:s');
[/insert_php]

[insert_php]
echo 'fwfwfw ';
[/insert_php]

[insert_php]
$host = "localhost";
$username = "root";
$password = "FIT5120lumus";
$dbname = "test";
$connection = mysql_connect($host, $username, $password, $dbname);
[/insert_php]

[insert_php]
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