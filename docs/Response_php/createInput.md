## Response->createInput()

####Signature: public function createInput($sParent, $sType, $sName, $sId)

####Parameters:

* $sParent The id of the parent element

* $sType The type of the new input element

* $sName The name of the new input element

* $sId The id of the new element

####Source Comments:

Add a command to create an input element on the browser  

return \Xajax\Plugin\Response
>


####Writers Description:
Use to add an input element to the html of the page.

####Example:
```
function createInputExample()
{
    $oResponse = new Response()
    $oResponse->createInput('theParent','button','newbuttonid', newbuttonname');
    return $oResponse
}
```