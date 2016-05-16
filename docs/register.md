## Xajax->register()

Signature: public function register($sType, $mArg)

Parameters:

* $sType

* $mArg




Source Comments:

Register request handlers, including functions, callable objects and events.



New plugins can be added that support additional registration methods and request processors.





param string	$sType			The type of request handler being registered

Options include:

- Xajax::USER_FUNCTION: a function declared at global scope

- Xajax::CALLABLE_OBJECT: an object who's methods are to be registered

- Xajax::BROWSER_EVENT: an event which will cause zero or more event handlers to be called

- Xajax::EVENT_HANDLER: register an event handler function.

param mixed		$sFunction | $objObject | $sEvent

When registering a function, this is the name of the function

When registering a callable object, this is the object being registered

When registering an event or event handler, this is the name of the event

param midex		$sIncludeFile | $aCallOptions | $sEventHandler

When registering a function, this is the (optional) include file

When registering a callable object, this is an (optional) array

of call options for the functions being registered

When registering an event handler, this is the name of the function



return mixed



Description:


Example:
<code><pre>
function registerExample()
{
	$xajax->register();
}
</pre></code>