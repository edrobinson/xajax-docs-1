## Response->removeCSS()

####Signature: public function removeCSS($sFileName, $sMedia = null)

####Parameters:

* $sFileName The relative or fully qualified URI of the css file

* $sMedia = null




####Source Comments:

Add a command to remove a LINK reference to a CSS file on the browser

This causes the browser to unload the style sheet, effectively removing the style changes it caused.

return \Xajax\Plugin\Response

####Example:
```
function removeCSSExample()
{
    $oResponse = new Response();
    $oResponse->removeCSS('..styles/tempStyle.css');
    return $oResponse;
}
```