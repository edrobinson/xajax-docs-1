## Response->sendHeaders()

####Signature: public function sendHeaders()

####Parameters:


####Source Comments:

Used internally to generate the response headers



return void



####Description:


####Example:
<code><pre>
function sendHeadersExample()
{
    $oResponse = new Response()
    $oResponse->sendHeaders()
    return $oResponse
}
</pre></code>