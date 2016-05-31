## xajax->getConfiguration()

####Signature: public function getConfiguration($sName)

####Parameters:

* array	$sName The name of the configuration setting
* return mixed

####Source Comments:

Get the current value of a configuration setting  
This function is deprecated, and will be removed in a future version. Use **getOption** instead.
####Writers Description:
This is usually used internally but you can use it to retrieve some option.

####Example:
```
function getConfigurationExample()
{
	$opt = $xajax->getConfiguration('someOpt');
}
```