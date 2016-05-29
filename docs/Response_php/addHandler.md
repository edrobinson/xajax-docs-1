## Response->addHandler()

####Signature: public function addHandler($sTarget, $sEvent, $sHandler)

####Parameters:

* $sTarget

* $sEvent

* $sHandler




####Source Comments:

Add a command to install an event handler on the specified element.

You can add more than one event handler to an element's event using this method.

param string		$sTarget			The id of the element

param string		$sEvent				The name of the event

param string		$sHandler			The javascript function to call when the event is fired

return \Xajax\Plugin\Response

####Description:
Use this method to add an event handler to an element on the browser page.
Note that the event should not include the 'on' prefix. i.e. 'click' not
'onclick.'

####Example:
```
function addHandlerExample()
{
    $oResponse = new Response()
    $oResponse->addHandler('myinput','click','myInputClick')
    return $oResponse
}
```