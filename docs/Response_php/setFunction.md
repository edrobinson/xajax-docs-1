## Response->setFunction()

####Signature: public function setFunction($sFunction, $sArgs, $sScript)

####Parameters:

* $sFunction

* $sArgs

* $sScript




####Source Comments:

Add a command to construct a javascript function on the browser



param string		$sFunction			The name of the function to construct

param string		$sArgs				Comma separated list of parameter names

param string		$sScript			The javascript code that will become the body of the function



return \Xajax\Plugin\Response



####Description:


####Example:
```
function setFunctionExample()
{
    $oResponse = new Response()
    $oResponse->setFunction()
    return $oResponse
}
```