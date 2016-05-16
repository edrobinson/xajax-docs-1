## Xajax->errorHandler()

Signature: public function errorHandler($errno, $errstr, $errfile, $errline)

Parameters:

* $errno

* $errstr

* $errfile

* $errline




Source Comments:

This function is registered with PHP's set_error_handler if the xajax error handling system is enabled



return void



Description:


Example:
<code><pre>
function errorHandlerExample()
{
	$xajax->errorHandler();
}
</pre></code>