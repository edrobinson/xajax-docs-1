## Response->removeHandler()

Signature: public function removeHandler($sTarget, $sEvent, $sHandler)

Parameters:

* $sTarget
* $sEvent
* $sHandler

Description:

Response command used to remove an event handler from an element.

Parameters:

sTarget - (string):  The id of the element.
sEvent - (string):  The name of the event.
sHandler - (string):  The javascript function that is called when the
event is fired.

Returns:

object : The <Response> object.

Example:
<code><pre>
function removeHandlerExample()
{
    $oResponse = new Response()
    $oResponse->removeHandler()
    return $oResponse
}
</pre></code>