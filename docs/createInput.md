## Response->createInput()

Signature: public function createInput($sParent, $sType, $sName, $sId)

Parameters:

* $sParent
* $sType
* $sName
* $sId

Description:

Response command used to create an input element on the browser.

Parameters:

sParent - (string):  The id of the parent element.
sType - (string):  The type of the new input element.
sName - (string):  The name of the new input element.
sId - (string):  The id of the new element.

Returns:

object : The <Response> object.

Example:
<code><pre>
function createInputExample()
{
    $oResponse = new Response()
    $oResponse->createInput()
    return $oResponse
}
</pre></code>