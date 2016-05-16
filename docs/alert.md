## Response->alert()

Signature: public function alert($sMsg)

Parameters:

* $sMsg

Description:

Response command that is used to display an alert message to the user.

Parameters:

sMsg - (string):  The message to be displayed.

Returns:

object : The <Response> object.

Example:
<code><pre>
function alertExample()
{
    $oResponse = new Response()
    $oResponse->alert()
    return $oResponse
}
</pre></code>