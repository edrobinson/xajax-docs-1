## xajax->disableAutoLoad()

####Signature: public function disableAutoLoad()
####Source Comments:
Disable the PHP class autoloader.. 

return void
####Writers Description:
If for some reason you need to disable the autoloading features of this Xajax version, this is the place to call.

####Example:
```
function disableAutoLoadExample()
{
	$xajax->disableAutoLoad();
}
```