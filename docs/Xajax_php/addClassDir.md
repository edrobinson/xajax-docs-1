## xajax->addClassDir()

####Signature: public function addClassDir($sPath, $sNamespace = null, array $aExcluded = array())

####Parameters:

* string $sPath The path to the directory

* string|null $sNamespace The associated namespace

* array $aExcluded These methods will not be registered
* return boolean

####Source Comments:

Add a path to the class directories

####Example:
```
function addClassDirExample()
{
	$xajax->addClassDir();
}
```