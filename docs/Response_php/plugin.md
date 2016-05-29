## Response->plugin()

####Signature: public function plugin($sName)

####Parameters:

* $sName The name of the plugin obj.

####Source Comments:

Provides access to registered response plugins  
Pass the plugin name as the first argument and the plugin object will be returned.

You can then access the methods of the plugin directly.  
return \Xajax\Plugin\Response
####Example:
```
function pluginExample()
{
    $oResponse = new Response;
    $oPlugin = $oResponse->plugin('myplugin');  //Get a reference to the plugin
    $oPlugin->setSomething('aaa');  //Invoke one of the plugin methods
}
```