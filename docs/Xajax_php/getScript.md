## xajax->getScript()

####Signature: public function getScript($bIncludeJs = false, $bIncludeCss = false)

####Parameters:
<pre>

* $bIncludeJs = false

* $bIncludeCss = false



</pre>
####Source Comments:
<pre>

Returns the Xajax Javascript header and wrapper code to be printed into the page



The javascript code returned by this function is dependent on the plugins

that are included and the functions and classes that are registered.



param boolean		$bIncludeJs			Also get the JS files

param boolean		$bIncludeCss		Also get the CSS files



return string


</pre>
####Description:


####Example:
<code><pre>
function getScriptExample()
{
	$xajax->getScript();
}
</pre></code>