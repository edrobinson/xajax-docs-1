## xajax->exportJavascript()

####Signature: public function exportJavascript($sJsAppDir, $sJsAppURI, $bMinifyJs = true)

####Parameters:
<pre>

* $sJsAppDir

* $sJsAppURI

* $bMinifyJs = true



</pre>
####Source Comments:
<pre>

Export and minify the javascript code generated by Xajax



param string		$sJsAppDir			The dir where the generated file will be located

param string		$sJsAppURI			The URI where the generated file will be located

param boolean		$bMinifyJs			Shall the generated file also be minified



return void


</pre>
####Description:


####Example:
<code><pre>
function exportJavascriptExample()
{
	$xajax->exportJavascript();
}
</pre></code>