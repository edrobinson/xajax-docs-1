## Response->removeScript()

####Signature: public function removeScript($sFileName, $sUnload = '')

####Parameters:

* $sFileName The relative or fully qualified URI of the javascript

* $sUnload = '' Name of a javascript function to call prior to unlaoding
* return \Xajax\Plugin\Response

####Source Comments:

Add a command to remove a SCRIPT reference to a javascript file on the browser

Optionally, you can call a javascript function just prior to the file being unloaded (for cleanup).

####Example:
```
function removeScriptExample()
{
    $oResponse = new Response()
    $oResponse->removeScript()
    return $oResponse
}
```