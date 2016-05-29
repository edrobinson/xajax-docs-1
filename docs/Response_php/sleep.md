## Response->sleep()

####Signature: public function sleep($tenths)

####Parameters:

* param integer		$tenths				The number of 1/10ths of a second to sleep
* return \Xajax\Plugin\Response

####Source Comments:

Add a command to make Xajax to pause execution of the response commands,  
returning control to the browser so it can perform other commands asynchronously.

After the specified delay, Xajax will continue execution of the response commands.

####Example:
```
function sleepExample()
{
    $oResponse = new Response();
    $oResponse->sleep(20); //2 second delay
    return $oResponse
}
```