## xajax->printScript()

####Signature: public function printScript($bIncludeJs = false, $bIncludeCss = false)

####Parameters:

* boolean $bIncludeJs Also print the JS files
* boolean $bIncludeCss Also print the CSS files
* return void

####Source Comments:
Print the xajax Javascript header and wrapper code into your page
The javascript code returned by this function is dependent on the plugins
that are included and the functions and classes that are registered.
####Writers Description:
This method prints the output from getScript().
Use it in the html source.

####Example:
```
<?php
	$xajax->printScript();
?>
```