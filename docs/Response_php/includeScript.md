## Response->includeScript()

####Signature: public function includeScript($sFileName, $sType = null, $sId = null)

####Parameters:

* $sFileName The relative or fully qualified URI of the javascript file

* $sType = null Defaults to text/javascript

* $sId = null

####Source Comments:

Add a command to load a javascript file on the browser  
return \Xajax\Plugin\Response

####Description:
This causes a JS script to be loaded on the browser.  
It's contents are immediately available and anything outside of a function
is executed.
####Example:
```
function includeScriptExample()
{
    $oResponse = new Response()
    $oResponse->includeScript('scripts/specialJs.js');
    return $oResponse
}
```