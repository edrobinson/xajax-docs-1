## Response->create()

Signature: public function create($sParent, $sTag, $sId)

Parameters:

* $sParent
* $sTag
* $sId

Description:

Response command used to create a new element on the browser.

Parameters:

sParent - (string):  The id of the parent element.
sTag - (string):  The tag name to be used for the new element.
sId - (string):  The id to assign to the new element.


Returns:

object : The <Response> object.

Example:
<code><pre>
function createExample()
{
    $oResponse = new Response()
    $oResponse->create()
    return $oResponse
}
</pre></code>