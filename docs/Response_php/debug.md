## Response->debug()

####Signature: public function debug($sMessage)

####Parameters:

* $sMessage




####Source Comments:

Add a command to display a debug message to the user



param string		$sMessage			The message to be displayed



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function debugExample()
{
    $oResponse = new Response()
    $oResponse->debug()
    return $oResponse
}
</pre></code>