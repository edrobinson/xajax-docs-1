## Response->setReturnValue()

####Signature: public function setReturnValue($value)

####Parameters:

* $value Any value
* return \Xajax\Plugin\Response

####Source Comments:

Stores a value that will be passed back as part of the response  
When making synchronous requests, the calling javascript can obtain this value  
immediately as the return value of the <xajax.call> javascript function

####Writers Description:
This is the mechanism used to return a single value when using the sychronous  
mode wherein the browser blocks until the response is received from the server.

The value can a number or string or whatever the callingfunction is expecting.

####Example:
```
function setReturnValueExample()
{
    $oResponse = new Response();
    $oResponse->setReturnValue(123.55);
    return $oResponse;
}
```