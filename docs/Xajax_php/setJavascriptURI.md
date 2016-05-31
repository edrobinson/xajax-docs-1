## xajax->setJavascriptURI()

####Signature: public function setJavascriptURI($sJsLibURI)

####Parameters:
* string $sJsLibURI The URI of the Xajax javascript library files
* return void

####Source Comments:
Set the URI of the Xajax javascript library files
####Writers Description:
If you use a local copy of the xajax Javascript files, use this method to tell Xajax where the files are located.

####Example:
```
	$xajax->setJavascriptURI('xajax/');
```