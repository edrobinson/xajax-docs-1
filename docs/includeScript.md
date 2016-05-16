## Response->includeScript()

Signature: public function includeScript($sFileName, $sType = null, $sId = null)

Parameters:

* $sFileName
* $sType = null
* $sId = null

Description:

Response command used to load a javascript file on the browser.

Parameters:

sFileName - (string):  The relative or fully qualified URI of the
javascript file.

sType - (string): Determines the script type . Defaults to 'text/javascript'.


Returns:

object : The <Response> object.

Example:
<code><pre>
function includeScriptExample()
{
    $oResponse = new Response()
    $oResponse->includeScript()
    return $oResponse
}
</pre></code>