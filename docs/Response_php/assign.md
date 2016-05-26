## Response->assign()

####Signature: public function assign($sTarget, $sAttribute, $sData)

####Parameters:

* $sTarget

* $sAttribute

* $sData




####Source Comments:

Add a command to assign the specified value to the given element's attribute



param string		$sTarget			The id of the html element on the browser

param string		$sAttribute			The attribute to be assigned

param string		$sData				The value to be assigned to the attribute



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function assignExample()
{
    $oResponse = new Response()
    $oResponse->assign()
    return $oResponse
}
</pre></code>