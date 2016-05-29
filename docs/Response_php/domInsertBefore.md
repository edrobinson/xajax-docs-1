## Response->domInsertBefore()

####Signature: public function domInsertBefore($target, $variable)

####Parameters:

* $target

* $variable




####Source Comments:

Add a command to insert a DOM element before another



param string		$target				The DOM target element

param string		$variable			The DOM element name (id or class)



return \Xajax\Plugin\Response



####Writers Description:


####Example:
```
function domInsertBeforeExample()
{
    $oResponse = new Response()
    $oResponse->domInsertBefore()
    return $oResponse
}
```