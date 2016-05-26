## Response->wrapFunction()

####Signature: public function wrapFunction($sFunction, $sArgs, $aScripts, $sReturnValueVar)

####Parameters:

* $sFunction

* $sArgs

* $aScripts

* $sReturnValueVar




####Source Comments:

Add a command to construct a wrapper function around an existing javascript function on the browser



param string		$sFunction			The name of the existing function to wrap

param string		$sArgs				The comma separated list of parameters for the function

param array			$aScripts			An array of javascript code snippets that will be used to build

											the body of the function

											The first piece of code specified in the array will occur before

											the call to the original function, the second will occur after

											the original function is called.

param string		$sReturnValueVar	The name of the variable that will retain the return value

											from the call to the original function



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function wrapFunctionExample()
{
    $oResponse = new Response()
    $oResponse->wrapFunction()
    return $oResponse
}
</pre></code>