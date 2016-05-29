## Response->insertInput()

####Signature: public function insertInput($sBefore, $sType, $sName, $sId)

####Parameters:

* $sBefore The id of the element to be used as the reference point for the insertion

* $sType The type of the new input element

* $sName The name of the new input element

* $sId The id of the new element

####Source Comments:

Add a command to insert a new input element preceding the specified element

return \Xajax\Plugin\Response
####Example:
```
function insertInputExample()
{
    $oResponse = new Response()
    $oResponse->insertInput('Id1', 'checkbox','pizza','cheese');
    return $oResponse
}
```