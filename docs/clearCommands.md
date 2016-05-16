## Response->clearCommands()

Signature: public function clearCommands()

Parameters:

Description:

Clear all the commands already added to the response.

Returns:

object : The <Response> object.

Example:
<code><pre>
function clearCommandsExample()
{
    $oResponse = new Response()
    $oResponse->clearCommands()
    return $oResponse
}
</pre></code>