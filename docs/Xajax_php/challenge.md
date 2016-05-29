## xajax->challenge()

####Signature: public function challenge($algo=null, $value=null)

####Parameters:
<pre>

* $algo=null

* $value=null



</pre>
####Source Comments:
<pre>

Introduce a challenge and response cycle into the request response process



Sessions must be enabled to use this feature.



param string		$algo				The algorithm to use

param integer		$value				The value to hash



return void


</pre>
####Writers Description:


####Example:
```
function challengeExample()
{
	$xajax->challenge();
}
```