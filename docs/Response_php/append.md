## Response->append()

####Signature: public function append($sTarget, $sAttribute, $sData)

####Parameters:

* $sTarget

* $sAttribute

* $sData




####Source Comments:

Add a command to append the specified data to the given element's attribute



param string		$sTarget			The id of the element to be updated

param string		$sAttribute			The name of the attribute to be appended to

param string		$sData				The data to be appended to the attribute



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function appendExample()
{
    $oResponse = new Response()
    $oResponse->append()
    return $oResponse
}
</pre></code>