## Response->insertAfter()

Signature: public function insertAfter($sAfter, $sTag, $sId)

Parameters:

* $sAfter
* $sTag
* $sId

Description:

Response command used to insert a new element after the specified
one.

Parameters:

sAfter - (string):  The id of the element that will be used as a reference
for the insertion.
sTag - (string):  The tag name to be used for the new element.
sId - (string):  The id to be used for the new element.

Returns:

object : The <Response> object.

Example:
<code><pre>
function insertAfterExample()
{
    $oResponse = new Response()
    $oResponse->insertAfter()
    return $oResponse
}
</pre></code>