## xajax->challenge()

####Signature: public function challenge($algo=null, $value=null)

####Parameters:
* string $algo The algorithm to use

* integer $value The value to hash

* return void

####Source Comments:

Introduce a challenge and response cycle into the request response process

Sessions must be enabled to use this feature.

####Writers Description:
Use CRA security


####Example:
```
function challengeExample()
{
	$xajax->challenge();
}
```