## xajax->configure()

####Signature: public function configure($sName, $xValue)

####Parameters:
* string $sName The name of the configuration setting

* mixed $xValue The value of the setting

* return void

####Source Comments:
Set a configuration option

This function is deprecated, and will be removed in a future version. Use setOption instead.

####Writers Description:
This is the old configuration setting method. Try not to use it.

####Example:
```
function configureExample()
{
	$xajax->configure($optName, $optValue);
}
```