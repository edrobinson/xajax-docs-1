## Response->getContentType()

####Signature: public function getContentType()

####Parameters:


####Source Comments:

Get the content type, which is always set to 'application/json'



return string



####Description:


####Example:
<code><pre>
function getContentTypeExample()
{
    $oResponse = new Response()
    $oResponse->getContentType()
    return $oResponse
}
</pre></code>