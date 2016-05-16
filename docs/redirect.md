## Response->redirect()

Signature: public function redirect($sURL, $iDelay=0)

Parameters:

* $sURL
* $iDelay=0

Description:

Response command that causes the browser to navigate to the specified
URL.

Parameters:

sURL - (string):  The relative or fully qualified URL.
iDelay - (integer, optional):  Number of seconds to delay before
the redirect occurs.

Returns:

object : The <Response> object.

Example:
<code><pre>
function redirectExample()
{
    $oResponse = new Response()
    $oResponse->redirect()
    return $oResponse
}
</pre></code>