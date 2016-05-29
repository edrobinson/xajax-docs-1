## Response->confirmCommands()

####Signature: public function confirmCommands($iCmdNumber, $sMessage)

####Parameters:

* $iCmdNumber The number of commands to skip upon cancel

* $sMessage The message to display to the user
* return \Xajax\Plugin\Response

####Source Comments:

Response command that prompts user with [ok] [cancel] style message box.  
If the user clicks cancel, the specified number of response commands
following this one, will be skipped.

####Writers Description:
Use confirm to present a standard confirm dialog with a message and OK and Cancel buttons.
The first parameter is the number of commands to skip when the user clicks Cancel. 

In the example below the xajax_doSomethingDangerous function will be called if the user clicks the OK button. If Cancel is clicked, the call will not be made.

Useful for confirmation of a user's request to empty their database, for example.
####Example:
<pre>
function confirmCommandsExample()
{
    $oResponse = new Response()
    $oResponse->confirmCommands(1, 'Are you sure?');
    $oResponse->call(xajax_doSomethingDangerous');
    return $oResponse
}
</pre>