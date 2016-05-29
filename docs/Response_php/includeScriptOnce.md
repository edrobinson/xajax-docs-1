## Response->includeScriptOnce()

####Signature: public function includeScriptOnce($sFileName, $sType = null, $sId = null)

####Parameters:

* $sFileName The relative or fully qualified URI of the javascript

* $sType = null Determines the script type. Defaults to 'text/javascript'

* $sId = null




####Source Comments:

Add a command to include a javascript file on the browser if it has not already been loaded

return \Xajax\Plugin\Response

####Description:
This is like the includeScript method except that if the script is
already present there is no attempt to add it again.

####Example:
```
function includeScriptOnceExample()
{
    $oResponse = new Response()
    $oResponse->includeScriptOnce('scripts/anotherJsFile.js');
    return $oResponse
}
```