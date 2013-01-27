PHP-array-to-xml
================

convert array to xml on php.

You can use it like that

<?php
require_once("../../private/class/A2Xml.php");

@header("Content-type:application/xml");

$test['string']='文本'; 
$test['ss']='12:30'; 
$test[123]=123123123;
$test['asdasd']=true;
$test[3]=array(
  'entree'=>"salad\n;s<>s;#$$123123sss", 
	'maincourse'=>'steak'
);
echo xml_encode((object)$test,"hash");
?>

Here is the article explain it.

http://blog.waaile.com/array-to-xml/
