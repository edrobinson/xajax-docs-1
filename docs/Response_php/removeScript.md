## Response->removeScript()

####Signature: public function removeScript($sFileName, $sUnload = '')

####Parameters:

* $sFileName

* $sUnload = ''




####Source Comments:

Add a command to remove a SCRIPT reference to a javascript file on the browser



Optionally, you can call a javascript function just prior to the file being unloaded (for cleanup).



param string		$sFileName			The relative or fully qualified URI of the javascript file

param string		$sUnload			Name of a javascript function to call prior to unlaoding the file



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function removeScriptExample()
{
    $oResponse = new Response()
    $oResponse->removeScript()
    return $oResponse
}
</pre></code>