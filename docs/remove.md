## Response->remove()

Signature: public function remove($sTarget)

Parameters:

* $sTarget

Description:

Response command used to remove an element from the document.

Parameters:

sTarget - (string):  The id of the element to be removed.

Returns:

object : The <Response> object.

Example:
<code><pre>
function removeExample()
{
    $oResponse = new Response()
    $oResponse->remove()
    return $oResponse
}
</pre></code>