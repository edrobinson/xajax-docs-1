## Response->setEvent()

Signature: public function setEvent($sTarget, $sEvent, $sScript)

Parameters:

* $sTarget
* $sEvent
* $sScript

Description:

Response command used to set an event handler on the browser.

Parameters:

sTarget - (string):  The id of the element that contains the event.
sEvent - (string):  The name of the event.
sScript - (string):  The javascript to execute when the event is fired.

Returns:

object : The <Response> object.

Example:
<code><pre>
function setEventExample()
{
    $oResponse = new Response()
    $oResponse->setEvent()
    return $oResponse
}
</pre></code>