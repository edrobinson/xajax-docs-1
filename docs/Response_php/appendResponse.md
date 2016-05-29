## Response->appendResponse()

####Signature: public function appendResponse($mCommands, $bBefore = false)

####Parameters:

* $mCommands The Response object

* $bBefore = false Add the new commands to the beginning of the list
* return void

####Source Comments:

Merge the response commands from the specified Response object with  
the response commands in this Response object.

####Writers Description:
Using this method you can add response commands from another 
function during an xajax processed call. This can save calls
to the server by completing processing that would take 2 or
more calls.

####Example:
```
function appendResponseExample()
{
    $oResponse = new Response()
    $oResponse->appendResponse(someOtherFunction()) /someOther Function returns a response obj.
    return $oResponse
}
function someOtherFunction(){
    $oResponse = new Response()
    $oResponse->alert('Message from the dark side...');
    return $oResponse
}
```