## Response->appendResponse()

Signature: public function appendResponse($mCommands, $bBefore = false)

Parameters:

* $mCommands
* $bBefore = false

Description:

Merges the response commands from the specified <Response>
object with the response commands in this <Response> object.

Parameters:

mCommands - (object):  <Response> object.
bBefore - (boolean):  Add the new commands to the beginning
of the list.


Example:
<code><pre>
function appendResponseExample()
{
    $oResponse = new Response()
    $oResponse->appendResponse()
    return $oResponse
}
</pre></code>