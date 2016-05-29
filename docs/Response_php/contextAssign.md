## Response->contextAssign()

####Signature: public function contextAssign($sAttribute, $sData)

####Parameters:

* $sAttribute

* $sData




####Source Comments:

Add a command to assign a value to a member of a javascript object (or element)

that is specified by the context member of the request



The object is referenced using the 'this' keyword in the sAttribute parameter.



param string		$sAttribute			The attribute to be updated

param string		$sData				The value to assign



return \Xajax\Plugin\Response



####Writers Description:


####Example:
```
function contextAssignExample()
{
    $oResponse = new Response()
    $oResponse->contextAssign()
    return $oResponse
}
```