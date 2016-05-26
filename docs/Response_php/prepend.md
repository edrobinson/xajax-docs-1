## Response->prepend()

####Signature: public function prepend($sTarget, $sAttribute, $sData)

####Parameters:

* $sTarget

* $sAttribute

* $sData




####Source Comments:

Add a command to prepend the specified data to the given element's attribute



param string		$sTarget			The id of the element to be updated

param string		$sAttribute			The name of the attribute to be prepended to

param string		$sData				The value to be prepended to the attribute



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function prependExample()
{
    $oResponse = new Response()
    $oResponse->prepend()
    return $oResponse
}
</pre></code>