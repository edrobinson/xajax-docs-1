## Response->sleep()

####Signature: public function sleep($tenths)

####Parameters:

* $tenths




####Source Comments:

Add a command to make Xajax to pause execution of the response commands,

returning control to the browser so it can perform other commands asynchronously.



After the specified delay, Xajax will continue execution of the response commands.



param integer		$tenths				The number of 1/10ths of a second to sleep



return \Xajax\Plugin\Response



####Description:


####Example:
```
function sleepExample()
{
    $oResponse = new Response()
    $oResponse->sleep()
    return $oResponse
}
```