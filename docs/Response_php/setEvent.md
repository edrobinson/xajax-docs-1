## Response->setEvent()

####Signature: public function setEvent($sTarget, $sEvent, $sScript)

####Parameters:

* string $sTarget The id of the element that contains the event

* string $sEvent The name of the event

* string $sScript The javascript to execute when the event is fired
* return \Xajax\Plugin\Response




####Source Comments:

Add a command to set an event handler on the browser

####Example:
```
function setEventExample()
{
    $oResponse = new Response()
    $oResponse->setEvent()
    return $oResponse
}
```