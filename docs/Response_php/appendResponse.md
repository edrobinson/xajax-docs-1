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
Using this method you can add response commands from another 
function during an xajax processed call. This can save calls
to the server by completing processing that would take 2 or
more calls.

####Example:
<code>

function appendResponseExample()
{
    $oResponse = new Response()
    $oResponse->appendResponse(someOtherFunction())
    return $oResponse
}
function someOtherFunction(){
    $oResponse = new Response()
    $oResponse->alert('Message from the dark side...');
    return $oResponse
}
</code>