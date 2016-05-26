## Response->setEvent()

####Signature: public function setEvent($sTarget, $sEvent, $sScript)

####Parameters:

* $sTarget

* $sEvent

* $sScript




####Source Comments:

Add a command to set an event handler on the browser



param string		$sTarget			The id of the element that contains the event

param string		$sEvent				The name of the event

param string		$sScript			The javascript to execute when the event is fired



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function setEventExample()
{
    $oResponse = new Response()
    $oResponse->setEvent()
    return $oResponse
}
</pre></code>