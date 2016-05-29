## Response->domInsertAfter()

####Signature: public function domInsertAfter($target, $variable)

####Parameters:

* $target

* $variable




####Source Comments:

Add a command to insert a DOM element after another



param string		$target				The DOM target element

param string		$variable			The DOM element name (id or class)



return \Xajax\Plugin\Response



####Description:


####Example:
```
function domInsertAfterExample()
{
    $oResponse = new Response()
    $oResponse->domInsertAfter()
    return $oResponse
}
```