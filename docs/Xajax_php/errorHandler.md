## xajax->errorHandler()

####Signature: public function errorHandler($errno, $errstr, $errfile, $errline)

####Parameters:
<pre>

* $errno

* $errstr

* $errfile

* $errline



</pre>
####Source Comments:
<pre>

This function is registered with PHP's set_error_handler if the xajax error handling system is enabled



return void


</pre>
####Description:


####Example:
<code><pre>
function errorHandlerExample()
{
	$xajax->errorHandler();
}
</pre></code>