## xajax->processRequest()

####Signature: public function processRequest()

####Parameters:
<pre>

</pre>
####Source Comments:
<pre>

If this is a xajax request, call the requested PHP function, build the response and send it back to the browser



This is the main server side engine for xajax.

It handles all the incoming requests, including the firing of events and handling of the response.

If your RequestURI is the same as your web page, then this function should be called before ANY

headers or HTML is output from your script.



This function may exit after the request is processed, if the 'core.exit_after' option is set to true.



return void



see <Xajax\Xajax->canProcessRequest>


</pre>
####Writers Description:


####Example:
```
function processRequestExample()
{
	$xajax->processRequest();
}
```