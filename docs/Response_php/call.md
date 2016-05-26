## Response->call()

####Signature: public function call($sFunc)

####Parameters:

* $sFunc




####Source Comments:

Add a command to call the specified javascript function with the given (optional) parameters



param string		$sFunc				The name of the function to call



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function callExample()
{
    $oResponse = new Response()
    $oResponse->call()
    return $oResponse
}
</pre></code>