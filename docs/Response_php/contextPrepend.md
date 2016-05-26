## Response->contextPrepend()

####Signature: public function contextPrepend($sAttribute, $sData)

####Parameters:

* $sAttribute

* $sData




####Source Comments:

Add a command to prepend the speicified data to the given member of the current

javascript object specified by context in the current request



The object is access via the 'this' keyword in the sAttribute parameter.



param string		$sAttribute			The attribute to be updated

param string		$sData				The value to be prepended



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function contextPrependExample()
{
    $oResponse = new Response()
    $oResponse->contextPrepend()
    return $oResponse
}
</pre></code>