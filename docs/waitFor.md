## Response->waitFor()

Signature: public function waitFor($script, $tenths)

Parameters:

* $script
* $tenths

Description:

Response command instructing xajax to delay execution of the response
commands until a specified condition is met.  Note, this returns control
to the browser, so that other script operations can execute.  xajax
will continue to monitor the specified condition and, when it evaulates
to true, will continue processing response commands.

Parameters:

script - (string):  A piece of javascript code that evaulates to true
or false.
tenths - (integer):  The number of 1/10ths of a second to wait before
timing out and continuing with the execution of the response
commands.

Returns:

object : The <Response> object.

Example:
<code><pre>
function waitForExample()
{
    $oResponse = new Response()
    $oResponse->waitFor()
    return $oResponse
}
</pre></code>