## Response->clearCommands()

####Signature: public function clearCommands()

####Source Comments:
Clear all the commands already added to the response

return \Xajax\Plugin\Response



####Writers Description:
Although this is more for internal use, you could use it to remove the commands you have added to a Response object but it is more likely you would want to reconsider your code...

####Example:
```
function clearCommandsExample()
{
    $oResponse = new Response()
    $oResponse->alert('Don't Panic!');
    //You change your mind here
    $oResponse->clearCommands();
    $oResponse->alert('Go ahead and panic!');
    return $oResponse
}
```