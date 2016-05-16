## Response->prepend()

Signature: public function prepend($sTarget, $sAttribute, $sData)

Parameters:

* $sTarget
* $sAttribute
* $sData

Description:

Response command to prepend the specified value onto the given
element's property.

Parameters:

sTarget - (string):  The id of the element to be updated.
sAttribute - (string):  The property to be updated.
sData - (string):  The value to be prepended.

Returns:

object : The <Response> object.

Example:
<code><pre>
function prependExample()
{
    $oResponse = new Response()
    $oResponse->prepend()
    return $oResponse
}
</pre></code>