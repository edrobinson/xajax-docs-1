## Response->replace()

####Signature: public function replace($sTarget, $sAttribute, $sSearch, $sData)

####Parameters:

* $sTarget

* $sAttribute

* $sSearch

* $sData




####Source Comments:

Add a command to replace a specified value with another value within the given element's attribute



param string		$sTarget			The id of the element to update

param string		$sAttribute			The attribute to be updated

param string		$sSearch			The needle to search for

param string		$sData				The data to use in place of the needle



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function replaceExample()
{
    $oResponse = new Response()
    $oResponse->replace()
    return $oResponse
}
</pre></code>