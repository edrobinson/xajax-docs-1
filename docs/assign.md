## Response->assign()

Signature: public function assign($sTarget, $sAttribute, $sData)

Parameters:

* $sTarget
* $sAttribute
* $sData

Description:

Response command indicating that the specified value should be
assigned to the given element's attribute.

Parameters:

sTarget - (string):  The id of the html element on the browser.
sAttribute - (string):  The property to be assigned.
sData - (string):  The value to be assigned to the property.

Returns:

object : The <Response> object.


Example:
<code><pre>
function assignExample()
{
    $oResponse = new Response()
    $oResponse->assign()
    return $oResponse
}
</pre></code>