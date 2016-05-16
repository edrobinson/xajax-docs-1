## Xajax->plugin()

Signature: public function plugin($sName)

Parameters:

* $sName




Source Comments:

Return a registered response plugin



Pass the plugin name as the first argument and the plugin object will be returned.

You can then access the methods of the plugin directly.



param string		$sName				The plugin name



return \Xajax\Plugin\Response



Description:


Example:
<code><pre>
function pluginExample()
{
	$xajax->plugin();
}
</pre></code>