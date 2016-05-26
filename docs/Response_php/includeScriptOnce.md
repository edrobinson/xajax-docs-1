## Response->includeScriptOnce()

####Signature: public function includeScriptOnce($sFileName, $sType = null, $sId = null)

####Parameters:

* $sFileName

* $sType = null

* $sId = null




####Source Comments:

Add a command to include a javascript file on the browser if it has not already been loaded



param string		$sFileName			The relative or fully qualified URI of the javascript file

param string		$sType				Determines the script type. Defaults to 'text/javascript'



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function includeScriptOnceExample()
{
    $oResponse = new Response()
    $oResponse->includeScriptOnce()
    return $oResponse
}
</pre></code>