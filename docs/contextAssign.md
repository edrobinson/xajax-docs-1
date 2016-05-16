## Response->contextAssign()

Signature: public function contextAssign($sAttribute, $sData)

Parameters:

* $sAttribute
* $sData

Description:

Response command used to assign a value to a member of a
javascript object (or element) that is specified by the context
member of the request.  The object is referenced using the 'this' keyword
in the sAttribute parameter.

Parameters:

sAttribute - (string):  The property to be updated.
sData - (string):  The value to assign.

Returns:

object : The <Response> object.

Example:
<code><pre>
function contextAssignExample()
{
    $oResponse = new Response()
    $oResponse->contextAssign()
    return $oResponse
}
</pre></code>