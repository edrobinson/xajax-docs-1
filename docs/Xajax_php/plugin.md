## xajax->plugin()

####Signature: public function plugin($sName)

####Parameters:
* string $sName The plugin name
* return \Xajax\Plugin\Response
####Source Comments:
Return a registered response plugin
Pass the plugin name as the first argument and the plugin object will be returned.
You can then access the methods of the plugin directly.

####Writers Description:
Use this method if you need access to a plugin object.

####Example:
```
function pluginExample()
{
	$plg = $xajax->plugin();
	$plg->someMethod(...);
}
```