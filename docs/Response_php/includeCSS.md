## Response->includeCSS()

####Signature: public function includeCSS($sFileName, $sMedia = null)

####Parameters:

* $sFileName The relative or fully qualified URI of the css file

* $sMedia The media type of the CSS file. Defaults to 'screen' 




####Source Comments:

Add a command to include a LINK reference to the specified CSS file on the browser.
This will cause the browser to load and apply the style sheet.

return \Xajax\Plugin\Response

####Description:
Use this to add a new style sheet to the browser. The parameter is the file uri.
The second parameter is the media type. It defaults to screen type.

####Example:
```
function includeCSSExample()
{
    $oResponse = new Response()
    $oResponse->includeCSS('..styles/newcss.css');
    return $oResponse
}
```