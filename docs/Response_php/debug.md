## Response->debug()

####Signature: public function debug($sMessage)

####Parameters:

* $sMessage The message to be displayed

####Source Comments:

Add a command to display a debug message to the user

return \Xajax\Plugin\Response



####Description:
Appears to be an internal method not usually called by a user.

####Example:
```
function debugExample()
{
    $oResponse = new Response();
    $oResponse->debug('The world will end tomorrow!');
    return $oResponse;
}
```