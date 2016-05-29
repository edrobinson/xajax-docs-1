## Response->script()

####Signature: public function script($sJS)

####Parameters:

* $sJS The script to execute
* return \Xajax\Plugin\Response

####Source Comments:

Add a command to execute a portion of javascript on the browser.

The script runs in it's own context, so variables declared locally, using the 'var' keyword,
will no longer be available after the call.

To construct a variable that will be accessable globally, even after the script has executed,
leave off the 'var' keyword.

####Writers Description:
This lets you execute any js statement on the browser.

####Example:
```
function scriptExample()
{
    $oResponse = new Response;
    $oResponse->script("alert('This is a msg.')");
    $oResponse->script('doz = 12');
    return $oResponse;
}
```