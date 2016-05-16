## Xajax->getJavascript()

Signature: public function getJavascript($bIncludeAssets = true)

Parameters:

* $bIncludeAssets = true




Source Comments:

Returns the Xajax Javascript header and wrapper code to be printed into the page



The javascript code returned by this function is dependent on the plugins

that are included and the functions and classes that are registered.



param boolean		$bIncludeAssets		Also get the JS and CSS files



return string



Description:


Example:
<code><pre>
function getJavascriptExample()
{
	$xajax->getJavascript();
}
</pre></code>