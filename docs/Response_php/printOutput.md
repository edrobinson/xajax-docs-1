## Response->printOutput()

####Signature: public function printOutput()

####Parameters:


####Source Comments:

Print the output, generated from the commands added to the response, that will be sent to the browser



return void



####Description:


####Example:
```
function printOutputExample()
{
    $oResponse = new Response()
    $oResponse->printOutput()
    return $oResponse
}
```