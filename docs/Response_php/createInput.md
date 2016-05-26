## Response->createInput()

####Signature: public function createInput($sParent, $sType, $sName, $sId)

####Parameters:

* $sParent

* $sType

* $sName

* $sId




####Source Comments:

Add a command to create an input element on the browser



param string		$sParent			The id of the parent element

param string		$sType				The type of the new input element

param string		$sName				The name of the new input element

param string		$sId				The id of the new element



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function createInputExample()
{
    $oResponse = new Response()
    $oResponse->createInput()
    return $oResponse
}
</pre></code>