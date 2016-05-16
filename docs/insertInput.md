## Response->insertInput()

Signature: public function insertInput($sBefore, $sType, $sName, $sId)

Parameters:

* $sBefore
* $sType
* $sName
* $sId

Description:

Response command used to insert a new input element preceeding the
specified element.

Parameters:

sBefore - (string):  The id of the element to be used as the reference
point for the insertion.
sType - (string):  The type of the new input element.
sName - (string):  The name of the new input element.
sId - (string):  The id of the new input element.

Returns:

object : The <Response> object.

Example:
<code><pre>
function insertInputExample()
{
    $oResponse = new Response()
    $oResponse->insertInput()
    return $oResponse
}
</pre></code>