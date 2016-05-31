## xajax->getScript()

####Signature: public function getScript($bIncludeJs = false, $bIncludeCss = false)

####Parameters:
* boolean $bIncludeJs Also get the JS files

* boolean $bIncludeCss Also get the CSS files
* return string
####Source Comments:

Returns the Xajax Javascript header and wrapper code to be printed into the page.
The javascript code returned by this function is dependent on the plugins
that are included and the functions and classes that are registered.

Optionally you can get any additional JS and CSS by including the 2 booleans.
This maks it possible to get all output from Xajax in a singletrip to the server.
####Writers Description:
Use this method to retrieve the xajax Js and optionally other Js and Css.

####Example:
```
<?php
		echo $xajax->getScript();
?>
```