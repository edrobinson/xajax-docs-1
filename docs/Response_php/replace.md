## Response->replace()

####Signature: public function replace($sTarget, $sAttribute, $sSearch, $sData)

####Parameters:

* $sTarget The id of the element to update

* $sAttribute The attribute to be updated

* $sSearch The needle to search for

* $sData The data to use in place of the needle
* return \Xajax\Plugin\Response

####Source Comments:

Add a command to replace a specified value with another value within the given element's attribute

####Example:
```
function replaceExample()
{
    $oResponse = new Response(;)
    $oResponse->replace($id,'style','color','green');
    return $oResponse;
}
```