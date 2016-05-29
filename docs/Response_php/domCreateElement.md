## Response->domCreateElement()

####Signature: public function domCreateElement($variable, $tag)

####Parameters:

* $variable

* $tag




####Source Comments:

Add a command to create a DOM element



param string		$variable			The DOM element name (id or class)

param string		$tag				The HTML tag of the new DOM element



return \Xajax\Plugin\Response



####Writers Description:


####Example:
```
function domCreateElementExample()
{
    $oResponse = new Response()
    $oResponse->domCreateElement()
    return $oResponse
}
```