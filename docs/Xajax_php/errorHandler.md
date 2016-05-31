## xajax->errorHandler()

####Signature: public function errorHandler($errno, $errstr, $errfile, $errline)

####Parameters:
<pre>

* $errno

* $errstr

* $errfile

* $errline

* return void

</pre>
####Source Comments:
This function is registered with PHP's set_error_handler if the xajax error handling system is enabled
####Writers Description:
This is the Xajax internal error handler.

####Example:
```
function errorHandlerExample()
{
	$xajax->errorHandler();
}
```