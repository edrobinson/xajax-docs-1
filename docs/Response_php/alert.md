## Response->alert()

####Signature: public function alert($sMessage)

####Parameters:

* $sMessage The message to be displayed
* return \Xajax\Plugin\Response

####Source Comments:

Add a command to display an alert message to the user

####Writers Description:
Use this method to send a JS alert message to the browser.

####Example:
```
function alertExample()
{
    $oResponse = new Response()
    $oResponse->alert('It worked!')
    return $oResponse
}
```