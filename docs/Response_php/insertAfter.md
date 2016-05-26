## Response->insertAfter()

####Signature: public function insertAfter($sAfter, $sTag, $sId)

####Parameters:

* $sAfter

* $sTag

* $sId




####Source Comments:

Add a command to insert a new element after the specified



param string		$sBefore			The id of the element used as a reference point for the insertion

param string		$sTag				The tag name to be used for the new element

param string		$sId				The id to assign to the new element



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function insertAfterExample()
{
    $oResponse = new Response()
    $oResponse->insertAfter()
    return $oResponse
}
</pre></code>