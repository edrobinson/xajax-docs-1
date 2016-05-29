## Response->setFunction()

####Signature: public function setFunction($sFunction, $sArgs, $sScript)

####Parameters:

* string $sFunction	 The name of the function to construct

* string $sArgs Comma separated list of parameter names

* string $sScript The javascript code that will become the body of the function
* return \Xajax\Plugin\Response

####Source Comments:

Add a command to construct a javascript function on the browser

####Writers Description:
You can use this to add a js function to the page on the fly.

####Example:
```
function setFunctionExample()
{
    $oResponse = new Response();
    $oResponse->setFunction('newFunct','p1','p2','return p1+p2;');
    return $oResponse;
}
```