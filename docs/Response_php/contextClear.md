## Response->contextClear()

####Signature: public function contextClear($sAttribute)

####Parameters:

* $sAttribute




####Source Comments:

Add a command to to clear the value of the attribute specified in the sAttribute parameter



The member is access via the 'this' keyword and can be used to update a javascript

object specified by context in the request parameters.



param string		$sAttribute			The attribute to be cleared



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function contextClearExample()
{
    $oResponse = new Response()
    $oResponse->contextClear()
    return $oResponse
}
</pre></code>