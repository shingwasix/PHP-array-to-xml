PHP-array-to-xml
================

convert array to xml on php.

You can use it like that

<?php<br/>
require_once("A2Xml.php");<br/>
<br/>
@header("Content-type:application/xml");<br/>
<br/>
$test['string']='文本'; <br/>
$test['ss']='12:30'; <br/>
$test[123]=123123123;<br/>
$test['asdasd']=true;<br/>
$test[3]=array(<br/>
  'entree'=>"salad\n;s<>s;#$$123123sss", <br/>
	'maincourse'=>'steak'<br/>
);<br/>
echo xml_encode((object)$test,"hash");<br/>
?><br/>

Here is the article explain it.

http://blog.waaile.com/array-to-xml/
