## Response->setFunction()

Signature: public function setFunction($sFunction, $sArgs, $sScript)

Parameters:

* $sFunction
* $sArgs
* $sScript

Description:

Response command used to construct a javascript function on the browser.

Parameters:

sFunction - (string):  The name of the function to construct.
sArgs - (string):  Comma separated list of parameter names.
sScript - (string):  The javascript code that will become the body of the
function.

Returns:

object : The <Response> object.

Example:
<code><pre>
function setFunctionExample()
{
    $oResponse = new Response()
    $oResponse->setFunction()
    return $oResponse
}
</pre></code>