## xajax->processRequest()

####Signature: public function processRequest()
####Source Comments:
If this is a xajax request, call the requested PHP function, build the response and send it back to the browser

This is the main server side engine for xajax.

It handles all the incoming requests, including the firing of events and handling of the response.

If your RequestURI is the same as your web page, then this function should be called before ANY
headers or HTML is output from your script.

This function may exit after the request is processed, if the 'core.exit_after' option is set to true.

see Xajax\Xajax->canProcessRequest
####Writers Description:
This is the main server side Xajax method. 

When called it determines if this is a page load or a request from the client. At page load it simply returns and lets the rest of the load complete. If, however, it determines that some plugin can handle the call it treats the event as a call from the client and makes the appropriate calls and returns to the client. All of this is invisible to the deeloper and is the real crux of Xajax.

Please note that any non-function code before the call to processRequest is always executed. Thus, only code that required at each load should be placedbefore the call. Code after the processRequest can be processed a page load but not during an incoming client request. 

Failure to adhere to this rule will lead to rather unpredictable results.

####Example:
```
<?php
    require (__DIR__ . './vendor/autoload.php');
    
    use Xajax\Xajax;
    use Xajax\Response\Response;
    
    $xajax = Xajax::getInstance();
    $xajax->register(XAJAX_FUNCTION,'myFunction');
    
    $_SESSION['EachTime'] = 0; //Happens at every call to this page...    

    $xajax->processRequest();
    
    $_SESSION['JustStarting'] = true; //Only happens once...
    
    function myFunction(){...};
    
```