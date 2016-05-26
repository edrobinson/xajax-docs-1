## Response->clearCommands()

####Signature: public function clearCommands()

####Parameters:


####Source Comments:

Clear all the commands already added to the response



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function clearCommandsExample()
{
    $oResponse = new Response()
    $oResponse->clearCommands()
    return $oResponse
}
</pre></code>