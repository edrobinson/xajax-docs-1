## Response->insert()

Signature: public function insert($sBefore, $sTag, $sId)

Parameters:

* $sBefore
* $sTag
* $sId

Description:

Response command used to insert a new element just prior to the specified
element.

Parameters:

sBefore - (string):  The element used as a reference point for the
insertion.
sTag - (string):  The tag to be used for the new element.
sId - (string):  The id to be used for the new element.

Returns:

object : The <Response> object.

Example:
<code><pre>
function insertExample()
{
    $oResponse = new Response()
    $oResponse->insert()
    return $oResponse
}
</pre></code>