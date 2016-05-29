## Response->insert()

####Signature: public function insert($sBefore, $sTag, $sId)

####Parameters:

* $sBefore The id of the element used as a reference point for the insertion

* $sTag The tag name to be used for the new element

* $sId The id to assign to the new element


####Source Comments:

Add a command to insert a new element just prior to the specified element

return \Xajax\Plugin\Response

####Example:
```
function insertExample()
{
    $oResponse = new Response()
    $oResponse->insert('myDiv', 'div','newDiv');
    return $oResponse
}
```