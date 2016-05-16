## Response->sleep()

Signature: public function sleep($tenths)

Parameters:

* $tenths

Description:

Response command which instructs xajax to pause execution
of the response commands, returning control to the browser
so it can perform other commands asynchronously.  After
the specified delay, xajax will continue execution of the
response commands.

Parameters:

tenths - (integer):  The number of 1/10ths of a second to
sleep.

Returns:

object : The <Response> object.

Example:
<code><pre>
function sleepExample()
{
    $oResponse = new Response()
    $oResponse->sleep()
    return $oResponse
}
</pre></code>