## Response->insertInput()

####Signature: public function insertInput($sBefore, $sType, $sName, $sId)

####Parameters:

* $sBefore

* $sType

* $sName

* $sId




####Source Comments:

Add a command to insert a new input element preceding the specified element



param string		$sBefore			The id of the element to be used as the reference point for the insertion

param string		$sType				The type of the new input element

param string		$sName				The name of the new input element

param string		$sId				The id of the new element



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function insertInputExample()
{
    $oResponse = new Response()
    $oResponse->insertInput()
    return $oResponse
}
</pre></code>