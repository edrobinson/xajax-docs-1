## Response->removeScript()

Signature: public function removeScript($sFileName, $sUnload = '')

Parameters:

* $sFileName
* $sUnload = ''

Description:

Response command used to remove a SCRIPT reference to a javascript
file on the browser.  Optionally, you can call a javascript function
just prior to the file being unloaded (for cleanup).

Parameters:

sFileName - (string):  The relative or fully qualified URI of the
javascript file.
sUnload - (string):  Name of a javascript function to call prior
to unlaoding the file.

Returns:

object : The <Response> object.

Example:
<code><pre>
function removeScriptExample()
{
    $oResponse = new Response()
    $oResponse->removeScript()
    return $oResponse
}
</pre></code>