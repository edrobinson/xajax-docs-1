Xajax is a PHP and Javascript library that takes the drudge out of using AJAX technology. The library has been around for over 10 years now and, despite a lag in development, it still has a faithful following.
  
Recently an enterprising user has taken on the task of updating and modernizing Xajax. Thanks to Mr. Thierry Feuzeu Xajax now consists of 2 packages; one for the server side and the other for client side.
   
The server side code is fully name spaced, uses autoloading and composer management. The Xajax plugin system has been overhauled to make it much more available and easier to develope in. The new Xajax requires a minimum of PHP 5.4 and works well with PHP 7.0 . The new code is available on [Github](https://github.com/lagdo/xajax-core). At present things are pretty much in the alpha state but soon we see a release a xajax 1.0.

Here is the traditional Hello World with Xajax:
   
**The PHP:**
```
<?php 
require (____DIR____ . '/xajax-core/vendor/autoload.php'); //Start autoload 
use Xajax\Xajax; //Use the xajax core clss
use Xajax\Response\Response; //and the Response class
$xajax = Xajax::getInstance();//Get the core singleton object   
//The function called by the browser
function helloworld($name) 
{ 
	$oresp = new Response(); 	  	//Instance the response class 
	$oresp->alert("Hello $name"); 	//Invoke the alert method to alert the user
	return $oresp;					//Return the response to the xajax engine 
}  
$xajax->register(XAJAX_FUNCTION,'helloworld'); //Register the function with Xajax 
$xajax->processRequest(); //Call the Xajax processing engine  
</code></pre>  
**The HTML:**
<pre><code>
&lt;!doctype html&gt;
&lt;html&gt;
&lt;head&gt;
	&lt;meta charset="utf-8"&gt;
	&lt;meta http-equiv="X-UA-Compatible" content="IE=edge"&gt;
	&lt;meta name="viewport" content="width=device-width, initial-scale=1"&gt;
	&lt;meta name="description" content=""&gt;
	&lt;meta name="author" content=""&gt;
	&lt;link rel="icon" href="/favicon.ico"&gt;
	&lt;title&gt;Xajax 0.7 Test&lt;/title&gt;
&lt;/head&gt;
&lt;body&gt;
	&lt;!-- The crux of this page --&gt;
	Enter your name:
	&lt;input type="text" name="username" id="username"/&gt;
	&lt;input type="button" value="Submit" onclick="xajax_helloworld(xajax.$('username').value)"/&gt;
	&lt;!-- Generate the xajax javascript--&gt;
	&lt;?php
		echo $xajax-&gt;getJsInclude();
		echo $xajax-&gt;getJavascript();
	?&gt;	
&lt;/body&gt;
&lt;/html&gt;
```

That's the basic Xajax page. There is a whole lot more so please study the documentation and give Xajax a try.
