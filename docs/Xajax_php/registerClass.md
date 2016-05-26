## xajax->registerClass()

####Signature: public function registerClass($sClassName, $bGetObject = false)

####Parameters:
<pre>

* $sClassName

* $bGetObject = false



</pre>
####Source Comments:
<pre>

Register a callable object from one of the class directories



The class name can be dot, slash or anti-slash separated.

If the $bGetObject parameter is set to true, the registered instance of the class is returned.



param string		$sClassName		The name of the class to register

param boolean		$bGetObject		Return the registered instance of the class



return void


</pre>
####Description:


####Example:
<code><pre>
function registerClassExample()
{
	$xajax->registerClass();
}
</pre></code>