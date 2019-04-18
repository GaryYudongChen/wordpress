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

<span class="vars">$mylink</span> = <span class="vars">$wpdb</span>-&gt;get_row(<span class="string">"SELECT * FROM $wpdb-&gt;Crops_Details WHERE Season = 'Summer'"</span>);

<span class="func">echo</span> <span class="vars">$mylink</span>-&gt;<span class="string">Season</span>;

[/insert_php]