## Response->includeCSS()

####Signature: public function includeCSS($sFileName, $sMedia = null)

####Parameters:

* $sFileName

* $sMedia = null




####Source Comments:

Add a command to include a LINK reference to the specified CSS file on the browser.



This will cause the browser to load and apply the style sheet.



param string		$sFileName			The relative or fully qualified URI of the css file

param string		$sMedia				The media type of the CSS file. Defaults to 'screen'



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function includeCSSExample()
{
    $oResponse = new Response()
    $oResponse->includeCSS()
    return $oResponse
}
</pre></code>