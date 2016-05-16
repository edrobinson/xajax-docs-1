## Response->contextAppend()

Signature: public function contextAppend($sAttribute, $sData)

Parameters:

* $sAttribute
* $sData

Description:

Response command used to append a value onto the specified member
of the javascript context object (or element) specified by the context
member of the request.  The object is referenced using the 'this' keyword
in the sAttribute parameter.

Parameters:

sAttribute - (string):  The member to be appended to.
sData - (string):  The value to append.

Returns:

object : The <Response> object.

Example:
<code><pre>
function contextAppendExample()
{
    $oResponse = new Response()
    $oResponse->contextAppend()
    return $oResponse
}
</pre></code>