## Response->call()

####Signature: public function call($sFunc)

####Parameters:

* $sFunc The name of the function to call
* return \Xajax\Plugin\Response

####Source Comments:

Add a command to call the specified javascript function with the given (optional) parameters

####Writers Description:
The call method is used to call a Javascript function on the browser.
Passing parameters is optional and they are passed as a comma seperated
list either variables or literals and numbers.

####Example:
```
function callExample()
{
    $oResponse = new Response()
    $oResponse->call('doSomethingSpecial',$p1,'param 2', 250);
    $oResponse->call('aSimpleFunction');
    return $oResponse
}
```