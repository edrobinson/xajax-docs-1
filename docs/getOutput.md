## Response->getOutput()

Signature: public function getOutput()

Parameters:

Description:

Returns the output, generated from the commands added to the response,
that will be sent to the browser.

Returns:

string : The textual representation of the response commands, in JSON format.

Example:
<code><pre>
function getOutputExample()
{
    $oResponse = new Response()
    $oResponse->getOutput()
    return $oResponse
}
</pre></code>