## Xajax->challenge()

Signature: public function challenge($algo=null, $value=null)

Parameters:

* $algo=null

* $value=null




Source Comments:

Introduce a challenge and response cycle into the request response process



Sessions must be enabled to use this feature.



param string		$algo				The algorithm to use

param integer		$value				The value to hash



return void



Description:


Example:
<code><pre>
function challengeExample()
{
	$xajax->challenge();
}
</pre></code>