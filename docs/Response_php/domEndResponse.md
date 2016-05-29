## Response->domEndResponse()

####Signature: public function domEndResponse()

####Parameters:


####Source Comments:

Add a command to end a DOM response



return \Xajax\Plugin\Response



####Writers Description:


####Example:
```
function domEndResponseExample()
{
    $oResponse = new Response()
    $oResponse->domEndResponse()
    return $oResponse
}
```