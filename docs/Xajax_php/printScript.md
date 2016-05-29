## xajax->printScript()

####Signature: public function printScript($bIncludeJs = false, $bIncludeCss = false)

####Parameters:
<pre>

* $bIncludeJs = false

* $bIncludeCss = false



</pre>
####Source Comments:
<pre>

Print the xajax Javascript header and wrapper code into your page



The javascript code returned by this function is dependent on the plugins

that are included and the functions and classes that are registered.



param boolean		$bIncludeJs			Also print the JS files

param boolean		$bIncludeCss		Also print the CSS files



return void


</pre>
####Writers Description:


####Example:
```
function printScriptExample()
{
	$xajax->printScript();
}
```