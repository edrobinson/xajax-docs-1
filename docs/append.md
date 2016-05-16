## Response->append()

Signature: public function append($sTarget, $sAttribute, $sData)

Parameters:

* $sTarget
* $sAttribute
* $sData

Description:

Response command that indicates the specified data should be appended
to the given element's property.

Parameters:

sTarget - (string):  The id of the element to be updated.
sAttribute - (string):  The name of the property to be appended to.
sData - (string):  The data to be appended to the property.

Returns:

object : The <Response> object.

Example:
<code><pre>
function appendExample()
{
    $oResponse = new Response()
    $oResponse->append()
    return $oResponse
}
</pre></code>