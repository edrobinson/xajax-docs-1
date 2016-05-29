## Response->removeHandler()

####Signature: public function removeHandler($sTarget, $sEvent, $sHandler)

####Parameters:

* $sTarget The id of the element

* $sEvent The name of the event

* $sHandler The javascript function called when the event is fired

####Source Comments:

Add a command to remove an event handler from an element.

return \Xajax\Plugin\Response

####Example:
```
function removeHandlerExample()
{
    $oResponse = new Response();
    $oResponse->removeHandler('goBtn','click','goClickService');
    return $oResponse;
}
```