## Response->remove()

####Signature: public function remove($sTarget)

####Parameters:

* $sTarget




####Source Comments:

Add a command to remove an element from the document



param string		$sTarget			The id of the element to be removed



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function removeExample()
{
    $oResponse = new Response()
    $oResponse->remove()
    return $oResponse
}
</pre></code>