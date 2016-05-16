## Response->clear()

Signature: public function clear($sTarget, $sAttribute)

Parameters:

* $sTarget
* $sAttribute

Description:

Response command used to clear the specified property of the
given element.

Parameters:

sTarget - (string):  The id of the element to be updated.
sAttribute - (string):  The property to be clared.

Returns:

object - The <Response> object.

Example:
<code><pre>
function clearExample()
{
    $oResponse = new Response()
    $oResponse->clear()
    return $oResponse
}
</pre></code>