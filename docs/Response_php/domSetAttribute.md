## Response->domSetAttribute()

####Signature: public function domSetAttribute($variable, $key, $value)

####Parameters:

* $variable

* $key

* $value




####Source Comments:

Add a command to set an attribute on a DOM element



param string		$variable			The DOM element name (id or class)

param string		$key				The name of the attribute

param string		$value				The value of the attribute



return \Xajax\Plugin\Response



####Writers Description:


####Example:
```
function domSetAttributeExample()
{
    $oResponse = new Response()
    $oResponse->domSetAttribute()
    return $oResponse
}
```