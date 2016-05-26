## Response->insertInputAfter()

####Signature: public function insertInputAfter($sAfter, $sType, $sName, $sId)

####Parameters:

* $sAfter

* $sType

* $sName

* $sId




####Source Comments:

Add a command to insert a new input element after the specified element



param string		$sAfter				The id of the element to be used as the reference point for the insertion

param string		$sType				The type of the new input element

param string		$sName				The name of the new input element

param string		$sId				The id of the new element



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function insertInputAfterExample()
{
    $oResponse = new Response()
    $oResponse->insertInputAfter()
    return $oResponse
}
</pre></code>