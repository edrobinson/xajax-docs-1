## Response->addPluginCommand()

####Signature: public function addPluginCommand($xPlugin, $aAttributes, $mData)

####Parameters:

* $xPlugin The plugin object

* $aAttributes The attributes for this response command

* $mData The data to be sent with this command
* return \Xajax\Plugin\Response

####Source Comments:
Add a response command that is generated by a plugin

####Example:
```
function addPluginCommandExample()
{
    $oResponse = new Response($xMyPlugin,$aAttributes,$mData);
    $oResponse->addPluginCommand();
    return $oResponse;
}
```