## Response->waitForCSS()

Signature: public function waitForCSS($iTimeout = 600)

Parameters:

* $iTimeout = 600

Description:

Response command instructing xajax to pause while the CSS
files are loaded.  The browser is not typically a multi-threading
application, with regards to javascript code.  Therefore, the
CSS files included or removed with <Response->includeCSS> and
<Response->removeCSS> respectively, will not be loaded or
removed until the browser regains control from the script.  This
command returns control back to the browser and pauses the execution
of the response until the CSS files, included previously, are
loaded.

Parameters:

iTimeout - (integer):  The number of 1/10ths of a second to pause
before timing out and continuing with the execution of the
response commands.

Returns:

object : The <Response> object.

Example:
<code><pre>
function waitForCSSExample()
{
    $oResponse = new Response()
    $oResponse->waitForCSS()
    return $oResponse
}
</pre></code>