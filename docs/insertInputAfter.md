## Response->insertInputAfter()

Signature: public function insertInputAfter($sAfter, $sType, $sName, $sId)

Parameters:

* $sAfter
* $sType
* $sName
* $sId

Description:

Response command used to insert a new input element after the
specified element.

Parameters:

sAfter - (string):  The id of the element that is to be used
as the insertion point for the new element.
sType - (string):  The type of the new input element.
sName - (string):  The name of the new input element.
sId - (string):  The id of the new input element.

Returns:

object : The <Response> object.

Example:
<code><pre>
function insertInputAfterExample()
{
    $oResponse = new Response()
    $oResponse->insertInputAfter()
    return $oResponse
}
</pre></code>