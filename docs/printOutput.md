## Response->printOutput()

Signature: public function printOutput()

Parameters:

Description:

Prints the output, generated from the commands added to the response,
that will be sent to the browser.

Example:
<code><pre>
function printOutputExample()
{
    $oResponse = new Response()
    $oResponse->printOutput()
    return $oResponse
}
</pre></code>