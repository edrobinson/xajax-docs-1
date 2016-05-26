## Response->confirmCommands()

####Signature: public function confirmCommands($iCmdNumber, $sMessage)

####Parameters:

* $iCmdNumber

* $sMessage




####Source Comments:

Response command that prompts user with [ok] [cancel] style message box



If the user clicks cancel, the specified number of response commands

following this one, will be skipped.



param integer		$iCmdNumber			The number of commands to skip upon cancel

param string		$sMessage			The message to display to the user



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function confirmCommandsExample()
{
    $oResponse = new Response()
    $oResponse->confirmCommands()
    return $oResponse
}
</pre></code>