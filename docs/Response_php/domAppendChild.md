## Response->domAppendChild()

####Signature: public function domAppendChild($parent, $variable)

####Parameters:

* $parent

* $variable




####Source Comments:

Add a command to append a child to a DOM element



param string		$parent				The DOM parent element

param string		$variable			The DOM element name (id or class)



return \Xajax\Plugin\Response



####Description:


####Example:
```
function domAppendChildExample()
{
    $oResponse = new Response()
    $oResponse->domAppendChild()
    return $oResponse
}
```