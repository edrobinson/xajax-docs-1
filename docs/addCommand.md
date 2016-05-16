## Response->addCommand()

Signature: public function addCommand($aAttributes, $mData)

Parameters:

* $aAttributes
* $mData

Description:

Add a response command to the array of commands that will
be sent to the browser.

Parameters:

aAttributes - (array):  Associative array of attributes that
will describe the command.
mData - (mixed):  The data to be associated with this command.

Returns:

object : The <Response> object.

Example:
<code><pre>
function addCommandExample()
{
    $oResponse = new Response()
    $oResponse->addCommand()
    return $oResponse
}
</pre></code>