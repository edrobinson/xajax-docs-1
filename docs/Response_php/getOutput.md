## Response->getOutput()

####Signature: public function getOutput()

####Parameters:


####Source Comments:

Return the output, generated from the commands added to the response, that will be sent to the browser



return string



####Description:


####Example:
<code><pre>
function getOutputExample()
{
    $oResponse = new Response()
    $oResponse->getOutput()
    return $oResponse
}
</pre></code>