## Response->waitFor()

####Signature: public function waitFor($script, $tenths)

####Parameters:

* string $script A piece of javascript code that evaulates to true or false

* integer $tenths The number of 1/10ths of a second to wait before timing out  
  and continuing with the execution of the response commands.
* return \Xajax\Plugin\Response




####Source Comments:

Add a command to make Xajax to delay execution of the response commands until a specified condition is met  
Note, this returns control to the browser, so that other script operations can execute.

Xajax will continue to monitor the specified condition and, when it evaulates to true,
will continue processing response commands.
####Example:
```
function waitForExample()
{
    $oResponse = new Response();
    $oResponse->waitFor(20); //Wait for 2 seconds
    return $oResponse;
}
```