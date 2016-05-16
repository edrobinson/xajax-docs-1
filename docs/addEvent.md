## Response->addEvent()

Signature: public function addEvent($sTarget, $sEvent, $sScript)

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

Note:

This function is depreciated and will be removed in a future version.
Use <setEvent> instead.

Example:
<code><pre>
function addEventExample()
{
    $oResponse = new Response()
    $oResponse->addEvent()
    return $oResponse
}
</pre></code>