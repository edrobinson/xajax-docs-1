## Response->domEndResponse()

####Signature: public function domEndResponse()

####Parameters:


####Source Comments:

Add a command to end a DOM response



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function domEndResponseExample()
{
    $oResponse = new Response()
    $oResponse->domEndResponse()
    return $oResponse
}
</pre></code>