## Response->getContentType()

####Signature: public function getContentType()

####Parameters:


####Source Comments:

Get the content type, which is always set to 'application/json'



return string



####Writers Description:


####Example:
```
function getContentTypeExample()
{
    $oResponse = new Response()
    $oResponse->getContentType()
    return $oResponse
}
```