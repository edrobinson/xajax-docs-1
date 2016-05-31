## xajax->canProcessRequest()

####Signature: public function canProcessRequest()
####Source Comments:
Determine if a call is a xajax request or a page load request
return boolean

####Writers Description:
This method simply determines if the incoming request is due to
an initial page load or is an xajax request from the browser.  
The method queries the plugin manager which, in turn, queries
all of the registered plugins. If no plugin can handle the request
it is treated as the page load event and false is returned.

####Example:
```
function canProcessRequestExample()
{
	$xajax->canProcessRequest();
}
```