## Response->sendHeaders()

Signature: public function sendHeaders()

Parameters:

Description:

Used internally to generate the response headers.

Example:
<code><pre>
function sendHeadersExample()
{
    $oResponse = new Response()
    $oResponse->sendHeaders()
    return $oResponse
}
</pre></code>