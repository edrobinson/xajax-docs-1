## Response->create()

####Signature: public function create($sParent, $sTag, $sId)

####Parameters:

* $sParent

* $sTag

* $sId




####Source Comments:

Add a command to create a new element on the browser



param string		$sParent			The id of the parent element

param string		$sTag				The tag name to be used for the new element

param string		$sId				The id to assign to the new element



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function createExample()
{
    $oResponse = new Response()
    $oResponse->create()
    return $oResponse
}
</pre></code>