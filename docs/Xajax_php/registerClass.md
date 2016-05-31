## xajax->registerClass()

####Signature: public function registerClass($sClassName, $bGetObject = false)

####Parameters:
* string $sClassName The name of the class to register

* boolean $bGetObject Return the registered instance of the class

* return void unless $bGetObject is true

####Source Comments:
Register a callable object from one of the class directories

The class name can be dot, slash or anti-slash separated.

If the $bGetObject parameter is set to true, the registered instance of the class is returned.
####Writers Description:


####Example:
```
function registerClassExample()
{
	$xajax->registerClass('classA');
}
```