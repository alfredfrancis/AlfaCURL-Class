AlfaCURL Class
==============

PHP class to perform cURL operations 

Examples
=========

1. To perform HTTP POST

```php
  <?
  include_once "alfa.curl.class.php";
  $curl=new AlfacURL();
	$post_data = "parameter1=value1&parameter2=value2";
	$url = "http://www.exaple.com/example.php";
	$ref="http://www.example.com";
	$content=($curl->post($url,$post_data,$ref));
	echo $content;
	?>
```
	
2. To perform HTTP GET

```php
  <?
  include_once "alfa.curl.class.php";
  $curl=new AlfacURL();
	$post_data = "parameter1=value1&parameter2=value2";
	$url = "http://www.exaple.com/example.php"."&".$post_data;
	$content=($curl->get($url));
	echo $content;
	?>
```
