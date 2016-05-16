## Xajax->addClassDir()

Signature: public function addClassDir($sPath, $sNamespace = null, array $aExcluded = array())

Parameters:

* $sPath

* $sNamespace = null

* array $aExcluded = array(




Source Comments:

Add a path to the class directories



param string		$sPath			The path to the directory

param string|null	$sNamespace		The associated namespace



return boolean



Description:


Example:
<code><pre>
function addClassDirExample()
{
	$xajax->addClassDir();
}
</pre></code>