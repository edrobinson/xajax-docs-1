## Response->wrapFunction()

Signature: public function wrapFunction($sFunction, $sArgs, $aScripts, $sReturnValueVariable)

Parameters:

* $sFunction
* $sArgs
* $aScripts
* $sReturnValueVariable

Description:

Response command used to construct a wrapper function around
and existing javascript function on the browser.

Parameters:

sFunction - (string):  The name of the existing function to wrap.
sArgs - (string):  The comma separated list of parameters for the function.
aScripts - (array):  An array of javascript code snippets that will
be used to build the body of the function.  The first piece of code
specified in the array will occur before the call to the original
function, the second will occur after the original function is called.
sReturnValueVariable - (string):  The name of the variable that will
retain the return value from the call to the original function.

Returns:

object : The <Response> object.

Example:
<code><pre>
function wrapFunctionExample()
{
    $oResponse = new Response()
    $oResponse->wrapFunction()
    return $oResponse
}
</pre></code>