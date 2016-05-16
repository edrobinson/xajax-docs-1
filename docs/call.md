## Response->call()

Signature: public function call() {

Parameters:

Description:

Response command that indicates that the specified javascript
function should be called with the given (optional) parameters.

Parameters:

arg1 - (string):  The name of the function to call.
arg2 .. argn : arguments to be passed to the function.

Returns:

object : The <Response> object.

Example:
<code><pre>
function callExample()
{
    $oResponse = new Response()
    $oResponse->call()
    return $oResponse
}
</pre></code>