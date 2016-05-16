## Response->confirmCommands()

Signature: public function confirmCommands($iCmdNumber, $sMessage)

Parameters:

* $iCmdNumber
* $sMessage

Description:

Response command that prompts user with [ok] [cancel] style
message box.  If the user clicks cancel, the specified
number of response commands following this one, will be
skipped.

Parameters:

iCmdNumber - (integer):  The number of commands to skip upon cancel.
sMessage - (string):  The message to display to the user.

Returns:

object : The Response object.

Example:
<code><pre>
function confirmCommandsExample()
{
    $oResponse = new Response()
    $oResponse->confirmCommands()
    return $oResponse
}
</pre></code>