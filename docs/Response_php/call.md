## Response->call()

####Signature: public function call($sFunc)

####Parameters:

* $sFunc

####Source Comments:

Add a command to call the specified javascript function with the given (optional) parameters

param string		$sFunc				The name of the function to call

return \Xajax\Plugin\Response

####Description:
The call method is usedto call a Javascript function on the browser.
Passing parameters is optional and they are passed as a comma seperated
list either variables or literals and numbers.

####Example:
<pre>
function callExample()
{
    $oResponse = new Response()
    $oResponse->call('doSomethingSpecial',$p1,'param 2');
    $oResponse->call('aSimpleFunction');
    return $oResponse
}
</pre>