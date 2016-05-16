## Response->includeCSS()

Signature: public function includeCSS($sFileName, $sMedia = null)

Parameters:

* $sFileName
* $sMedia = null

Description:

Response command used to include a LINK reference to
the specified CSS file on the browser.  This will cause the
browser to load and apply the style sheet.

Parameters:

sFileName - (string):  The relative or fully qualified URI of
the css file.

sMedia - (string): Determines the media type of the CSS file. Defaults to 'screen'.

Returns:

object : The <Response> object.

Example:
<code><pre>
function includeCSSExample()
{
    $oResponse = new Response()
    $oResponse->includeCSS()
    return $oResponse
}
</pre></code>