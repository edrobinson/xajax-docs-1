## Response->insertInputAfter()

####Signature: public function insertInputAfter($sAfter, $sType, $sName, $sId)

####Parameters:

* $sAfter The id of the element to be used as the reference point for the insertion

* $sType The type of the new input element

* $sName The name of the new input element

* $sId The id of the new element

####Source Comments:

Add a command to insert a new input element **after** the specified element

return \Xajax\Plugin\Response
####Example:
```
function insertInputAfterExample()
{
    $oResponse = new Response();
    $oResponse->insertInputAfter('div1','div','div2','div2');
    return $oResponse;
}
```