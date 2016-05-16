## Response->removeCSS()

Signature: public function removeCSS($sFileName, $sMedia = null)

Parameters:

* $sFileName
* $sMedia = null

Description:

Response command used to remove a LINK reference to
a CSS file on the browser.  This causes the browser to
unload the style sheet, effectively removing the style
changes it caused.

Parameters:

sFileName - (string):  The relative or fully qualified URI
of the css file.

Returns:

object : The <Response> object.

Example:
<code><pre>
function removeCSSExample()
{
    $oResponse = new Response()
    $oResponse->removeCSS()
    return $oResponse
}
</pre></code>