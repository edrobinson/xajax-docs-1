## Response->script()

Signature: public function script($sJS)

Parameters:

* $sJS

Description:

Response command that is used to execute a portion of javascript on
the browser.  The script runs in it's own context, so variables declared
locally, using the 'var' keyword, will no longer be available after the
call.  To construct a variable that will be accessable globally, even
after the script has executed, leave off the 'var' keyword.

Parameters:

sJS - (string):  The script to execute.

Returns:

object : The <Response> object.

Example:
<code><pre>
function scriptExample()
{
    $oResponse = new Response()
    $oResponse->script()
    return $oResponse
}
</pre></code>