## Response->contextClear()

Signature: public function contextClear($sAttribute)

Parameters:

* $sAttribute

Description:

Response command used to clear the value of the property specified
in the sAttribute parameter.  The member is access via the 'this'
keyword and can be used to update a javascript object specified
by context in the request parameters.

Parameters:

sAttribute - (string):  The member to be cleared.

Returns:

object : The <Response> object.

Example:
<code><pre>
function contextClearExample()
{
    $oResponse = new Response()
    $oResponse->contextClear()
    return $oResponse
}
</pre></code>