## Response->waitForCSS()

####Signature: public function waitForCSS($iTimeout = 600)

####Parameters:

* $iTimeout = 600
* return \Xajax\Plugin\Response

####Source Comments:

Add a command to make Xajax pause while the CSS files are loaded.  

The browser is not typically a multi-threading application, with regards to javascript code.  
Therefore, the CSS files included or removed with Response->includeCSS and Response->removeCSS respectively, will not be loaded or removed until the browser regains  control from the script.
This command returns control back to the browser and pauses the execution of the response until the CSS files, included previously, are loaded.

The timeout parameter specifies the number of 10ths of a second to pause before timing out and continuing with processing of the received response.

####Example:
```
function waitForCSSExample()
{
    $oResponse = new Response();
    $oResponse->waitForCSS(200);
    return $oResponse;
}
```