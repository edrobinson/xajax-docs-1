## Response->contextPrepend()

Signature: public function contextPrepend($sAttribute, $sData)

Parameters:

* $sAttribute
* $sData

Description:

Response command used to prepend the speicified data to the given
member of the current javascript object specified by context in the
current request.  The object is access via the 'this' keyword in the
sAttribute parameter.

Parameters:

sAttribute - (string):  The member to be updated.
sData - (string):  The value to be prepended.

Returns:

object : The <Response> object.

Example:
<code><pre>
function contextPrependExample()
{
    $oResponse = new Response()
    $oResponse->contextPrepend()
    return $oResponse
}
</pre></code>