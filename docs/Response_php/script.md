## Response->script()

####Signature: public function script($sJS)

####Parameters:

* $sJS




####Source Comments:

Add a command to execute a portion of javascript on the browser



The script runs in it's own context, so variables declared locally, using the 'var' keyword,

will no longer be available after the call.

To construct a variable that will be accessable globally, even after the script has executed,

leave off the 'var' keyword.



param string		$sJS				The script to execute



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function scriptExample()
{
    $oResponse = new Response()
    $oResponse->script()
    return $oResponse
}
</pre></code>