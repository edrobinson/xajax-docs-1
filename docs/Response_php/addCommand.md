## Response->addCommand()

####Signature: public function addCommand($aAttributes, $mData)

####Parameters:

* $aAttributes

* $mData




####Source Comments:

Add a response command to the array of commands that will be sent to the browser



param array 		$aAttributes		Associative array of attributes that will describe the command

param mixed			$mData				The data to be associated with this command



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function addCommandExample()
{
    $oResponse = new Response()
    $oResponse->addCommand()
    return $oResponse
}
</pre></code>