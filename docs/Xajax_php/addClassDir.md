## xajax->addClassDir()

####Signature: public function addClassDir($sPath, $sNamespace = null, array $aExcluded = array())

####Parameters:
<pre>

* $sPath

* $sNamespace = null

* array $aExcluded = array(



</pre>
####Source Comments:
<pre>

Add a path to the class directories



param string		$sPath			The path to the directory

param string|null	$sNamespace		The associated namespace



return boolean


</pre>
####Description:


####Example:
```
function addClassDirExample()
{
	$xajax->addClassDir();
}
```