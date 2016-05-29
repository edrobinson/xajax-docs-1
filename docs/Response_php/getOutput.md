## Response->getOutput()

####Signature: public function getOutput()

####Parameters:


####Source Comments:

Return the output, generated from the commands added to the response, that will be sent to the browser



return string



####Writers Description:


####Example:
```
function getOutputExample()
{
    $oResponse = new Response()
    $oResponse->getOutput()
    return $oResponse
}
```