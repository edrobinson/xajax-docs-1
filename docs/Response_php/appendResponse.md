## Response->appendResponse()

####Signature: public function appendResponse($mCommands, $bBefore = false)

####Parameters:

* $mCommands

* $bBefore = false




####Source Comments:

Merge the response commands from the specified <Response> object with

the response commands in this <Response> object



param Response		$mCommands			The <Response> object

param boolean		$bBefore			Add the new commands to the beginning of the list



return void



####Description:


####Example:
<code><pre>
function appendResponseExample()
{
    $oResponse = new Response()
    $oResponse->appendResponse()
    return $oResponse
}
</pre></code>