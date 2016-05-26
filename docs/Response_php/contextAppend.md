## Response->contextAppend()

####Signature: public function contextAppend($sAttribute, $sData)

####Parameters:

* $sAttribute

* $sData




####Source Comments:

Add a command to append a value onto the specified member of the javascript

context object (or element) specified by the context member of the request



The object is referenced using the 'this' keyword in the sAttribute parameter.



param string		$sAttribute			The attribute to be appended to

param string		$sData				The value to append



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function contextAppendExample()
{
    $oResponse = new Response()
    $oResponse->contextAppend()
    return $oResponse
}
</pre></code>