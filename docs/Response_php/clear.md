## Response->clear()

####Signature: public function clear($sTarget, $sAttribute)

####Parameters:

* $sTarget

* $sAttribute

####Source Comments:

Add a command to clear the specified attribute of the given element

* param string		$sTarget			The id of the element to be updated.
* param string		$sAttribute			The attribute to be cleared

return \Xajax\Plugin\Response
####Writers Description:
Use clear to remove or reset an attribute of an element. Useful for clearing
something like a readonly attribute.

####Example:
```
function clearExample()
{
    $oResponse = new Response()
    $oResponse->clear('targetId','height');
    return $oResponse
}
```