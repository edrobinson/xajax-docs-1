## Response->removeHandler()

####Signature: public function removeHandler($sTarget, $sEvent, $sHandler)

####Parameters:

* $sTarget

* $sEvent

* $sHandler




####Source Comments:

Add a command to remove an event handler from an element



param string		$sTarget			The id of the element

param string		$sEvent				The name of the event

param string		$sHandler			The javascript function called when the event is fired



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function removeHandlerExample()
{
    $oResponse = new Response()
    $oResponse->removeHandler()
    return $oResponse
}
</pre></code>