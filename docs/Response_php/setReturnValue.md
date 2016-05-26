## Response->setReturnValue()

####Signature: public function setReturnValue($value)

####Parameters:

* $value




####Source Comments:

Stores a value that will be passed back as part of the response



When making synchronous requests, the calling javascript can obtain this value

immediately as the return value of the <xajax.call> javascript function



param mixed		$value				Any value



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function setReturnValueExample()
{
    $oResponse = new Response()
    $oResponse->setReturnValue()
    return $oResponse
}
</pre></code>