## Response->alert()

####Signature: public function alert($sMessage)

####Parameters:

* $sMessage
####Source Comments:

Add a command to display an alert message to the user

param string		$sMessage			The message to be displayed

return \Xajax\Plugin\Response

####Description:
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