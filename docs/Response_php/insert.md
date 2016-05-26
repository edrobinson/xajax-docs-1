## Response->insert()

####Signature: public function insert($sBefore, $sTag, $sId)

####Parameters:

* $sBefore

* $sTag

* $sId




####Source Comments:

Add a command to insert a new element just prior to the specified element



param string		$sBefore			The id of the element used as a reference point for the insertion

param string		$sTag				The tag name to be used for the new element

param string		$sId				The id to assign to the new element



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function insertExample()
{
    $oResponse = new Response()
    $oResponse->insert()
    return $oResponse
}
</pre></code>