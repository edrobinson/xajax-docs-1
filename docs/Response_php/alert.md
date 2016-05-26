## Response->alert()

####Signature: public function alert($sMessage)

####Parameters:

* $sMessage




####Source Comments:

Add a command to display an alert message to the user



param string		$sMessage			The message to be displayed



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function alertExample()
{
    $oResponse = new Response()
    $oResponse->alert()
    return $oResponse
}
</pre></code>