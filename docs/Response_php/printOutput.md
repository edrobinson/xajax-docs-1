## Response->printOutput()

####Signature: public function printOutput()

####Parameters:


####Source Comments:

Print the output, generated from the commands added to the response, that will be sent to the browser



return void



####Description:


####Example:
<code><pre>
function printOutputExample()
{
    $oResponse = new Response()
    $oResponse->printOutput()
    return $oResponse
}
</pre></code>