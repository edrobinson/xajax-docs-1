## Response->insertAfter()

####Signature: public function insertAfter($sAfter, $sTag, $sId)

####Parameters:

* $sAfter The id of the element used as a reference point for the insertion

* $sTag The tag name to be used for the new element


* $sId The id to assign to the new element

####Source Comments:

Add a command to insert a new element after the specified

return \Xajax\Plugin\Response

####Example:
```
function insertAfterExample()
{
    $oResponse = new Response()
    $oResponse->insertAfter('existingId','div','newId');
    return $oResponse
}
```