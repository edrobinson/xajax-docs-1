## Response->domRemoveChildren()

####Signature: public function domRemoveChildren($parent, $skip = null, $remove = null)

####Parameters:

* $parent

* $skip = null

* $remove = null




####Source Comments:

Add a command to remove children from a DOM element



param string		$parent				The DOM parent element

param string		$skip				The ??

param string		$remove				The ??



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function domRemoveChildrenExample()
{
    $oResponse = new Response()
    $oResponse->domRemoveChildren()
    return $oResponse
}
</pre></code>