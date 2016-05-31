## xajax->configureMany()

####Signature: public function configureMany(array $aOptions)

####Parameters:
* array $aOptions Associative array of configuration settings
* return void

####Source Comments:
Set an array of configuration options
This function is deprecated, and will be removed in a future version. Use <setOptions> instead.
####Writers Description:
This is the old method of setting multiple options in one call. Use setOptions instead.

####Example:
```
function configureManyExample()
{
	$xajax->configureMany($aOptions);
}
```