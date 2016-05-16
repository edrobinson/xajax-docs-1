## Response->addHandler()

Signature: public function addHandler($sTarget, $sEvent, $sHandler)

Parameters:

* $sTarget
* $sEvent
* $sHandler

Description:

Response command used to install an event handler on the specified element.

Parameters:

sTarget - (string):  The id of the element.
sEvent - (string):  The name of the event to add the handler to.
sHandler - (string):  The javascript function to call when the event is fired.

You can add more than one event handler to an element's event using this method.

Returns:

object - The <Response> object.

Example:
<code><pre>
function addHandlerExample()
{
    $oResponse = new Response()
    $oResponse->addHandler()
    return $oResponse
}
</pre></code>