## Response->replace()

Signature: public function replace($sTarget, $sAttribute, $sSearch, $sData)

Parameters:

* $sTarget
* $sAttribute
* $sSearch
* $sData

Description:

Replace a specified value with another value within the given
element's property.

Parameters:

sTarget - (string):  The id of the element to update.
sAttribute - (string):  The property to be updated.
sSearch - (string):  The needle to search for.
sData - (string):  The data to use in place of the needle.

Example:
<code><pre>
function replaceExample()
{
    $oResponse = new Response()
    $oResponse->replace()
    return $oResponse
}
</pre></code>