## Response->plugin()

####Signature: public function plugin($sName)

####Parameters:

* $sName




####Source Comments:

Provides access to registered response plugins



Pass the plugin name as the first argument and the plugin object will be returned.

You can then access the methods of the plugin directly.



param string		$sName				The name of the plugin



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function pluginExample()
{
    $oResponse = new Response()
    $oResponse->plugin()
    return $oResponse
}
</pre></code>