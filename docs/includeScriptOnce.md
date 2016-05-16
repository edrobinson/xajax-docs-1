## Response->includeScriptOnce()

Signature: public function includeScriptOnce($sFileName, $sType = null, $sId = null)

Parameters:

* $sFileName
* $sType = null
* $sId = null

Description:

Response command used to include a javascript file on the browser
if it has not already been loaded.

Parameters:

sFileName - (string):  The relative for fully qualified URI of the
javascript file.

sType - (string): Determines the script type . Defaults to 'text/javascript'.

Returns:

object : The <Response> object.

Example:
<code><pre>
function includeScriptOnceExample()
{
    $oResponse = new Response()
    $oResponse->includeScriptOnce()
    return $oResponse
}
</pre></code>