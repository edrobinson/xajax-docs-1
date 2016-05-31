## xajax->register()

####Signature: public function register($sType, $mArg)

####Parameters:

* string $sType The type of request handler being registered

* mixed	$mArg $sFunction | $objObject | $sEvent
* return mixed

####Source Comments:

Register request handlers, including functions, callable objects and events.
New plugins can be added that support additional registration methods and request processors.

Parameter 1: $sType The type of request handler being registered

Options include:

* Xajax::USER_FUNCTION: a function declared at global scope

* Xajax::CALLABLE_OBJECT: an object who's methods are to be registered

* Xajax::BROWSER_EVENT: an event which will cause zero or more event handlers to be called

* Xajax::EVENT_HANDLER: register an event handler function.

Parameter 2: $sFunction | $objObject | $sEvent

* When registering a function, this is the name of the function

* When registering a callable object, this is the object being registered

* When registering an event or event handler, this is the name of the event

Optional Parameter 3: $sIncludeFile | $aCallOptions | $sEventHandler

* When registering a function, this is the (optional) include file

* When registering a callable object, this is an (optional) array
of call options for the functions being registered

* When registering an event handler, this is the name of the function

####Writers Description:
The register method tells xajax that you want to make a function or functions callable
from the browser. The most common usage is to register a single function to handle something on behalf of the user. An example would be to register new users when they submit the reg. form. The function is called in response to a submit button or a button type input and sends the reg. form fields using the xajax.getFormValues method.

The second type of registration call is used to register a class object's methods. You instance the class in question and use CALLABLE_OBJECT def. when calling register. Note that you do not use the class name but the object name. However, on the browser you call the methods using the class name.

This writer has had no experience with the BROWSER_EVENT or tne EVENT_HANDLER. It seems that they are supposed to provide server side event handling... 

####Example:
```
//Simple function regstration
//It registers "myFunction."
$xajax->register(Xajax::USER_FUNCTION, 'myFunction');

//Register a class object
class Utils{
  ...
} 
Utilities = new Utils;
$xajax->register(Xajax::CALLABLE_OBJECT,'Utilities');
```