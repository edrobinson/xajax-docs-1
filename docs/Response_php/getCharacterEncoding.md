## Response->getCharacterEncoding()

####Signature: public function getCharacterEncoding()

####Parameters:


####Source Comments:

Get the configured character encoding



return string



####Writers Description:


####Example:
```
function getCharacterEncodingExample()
{
    $oResponse = new Response()
    $oResponse->getCharacterEncoding()
    return $oResponse
}
```