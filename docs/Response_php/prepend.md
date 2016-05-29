## Response->prepend()

####Signature: public function prepend($sTarget, $sAttribute, $sData)

####Parameters:

* $sTarget The id of the element to be updated

* $sAttribute The name of the attribute to be prepended to

* $sData The value to be prepended to the attribute

####Source Comments:

Add a command to prepend the specified data to the given element's attribute

return \Xajax\Plugin\Response

####Description:


####Example:
```
function prependExample()
{
    $oResponse = new Response()
    $oResponse->prepend('name', 'value', 'Mr.'); //Prefix the value of name with Mr.
    return $oResponse
}
```