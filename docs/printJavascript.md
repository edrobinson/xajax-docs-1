## Xajax->printJavascript()

Signature: public function printJavascript()

Parameters:


Source Comments:

Print the xajax Javascript header and wrapper code into your page



The javascript code returned by this function is dependent on the plugins

that are included and the functions and classes that are registered.



return void



Description:


Example:
<code><pre>
function printJavascriptExample()
{
	$xajax->printJavascript();
}
</pre></code>