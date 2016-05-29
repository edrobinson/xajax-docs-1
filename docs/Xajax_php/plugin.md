## xajax->plugin()

####Signature: public function plugin($sName)

####Parameters:
<pre>

* $sName



</pre>
####Source Comments:
<pre>

Return a registered response plugin



Pass the plugin name as the first argument and the plugin object will be returned.

You can then access the methods of the plugin directly.



param string		$sName				The plugin name



return \Xajax\Plugin\Response


</pre>
####Writers Description:


####Example:
```
function pluginExample()
{
	$xajax->plugin();
}
```