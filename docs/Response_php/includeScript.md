## Response->includeScript()

####Signature: public function includeScript($sFileName, $sType = null, $sId = null)

####Parameters:

* $sFileName

* $sType = null

* $sId = null




####Source Comments:

Add a command to load a javascript file on the browser



param string		$sFileName			The relative or fully qualified URI of the javascript file

param string		$sType				Determines the script type. Defaults to 'text/javascript'



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function includeScriptExample()
{
    $oResponse = new Response()
    $oResponse->includeScript()
    return $oResponse
}
</pre></code>