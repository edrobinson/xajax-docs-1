## Response->removeCSS()

####Signature: public function removeCSS($sFileName, $sMedia = null)

####Parameters:

* $sFileName

* $sMedia = null




####Source Comments:

Add a command to remove a LINK reference to a CSS file on the browser



This causes the browser to unload the style sheet, effectively removing the style changes it caused.



param string		$sFileName			The relative or fully qualified URI of the css file



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function removeCSSExample()
{
    $oResponse = new Response()
    $oResponse->removeCSS()
    return $oResponse
}
</pre></code>