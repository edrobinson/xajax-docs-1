## Response->clear()

####Signature: public function clear($sTarget, $sAttribute)

####Parameters:

* $sTarget

* $sAttribute




####Source Comments:

Add a command to clear the specified attribute of the given element



param string		$sTarget			The id of the element to be updated.

param string		$sAttribute			The attribute to be cleared



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function clearExample()
{
    $oResponse = new Response()
    $oResponse->clear()
    return $oResponse
}
</pre></code>