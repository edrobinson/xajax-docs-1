## xajax->configure()

####Signature: public function configure($sName, $xValue)

####Parameters:
<pre>

* $sName

* $xValue



</pre>
####Source Comments:
<pre>

Set a configuration option



This function is deprecated, and will be removed in a future version. Use <setOption> instead.



param string 		$sName				The name of the configuration setting

param mixed			$xValue				The value of the setting



return void


</pre>
####Writers Description:


####Example:
```
function configureExample()
{
	$xajax->configure();
}
```