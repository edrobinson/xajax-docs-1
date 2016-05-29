## Response->domAppendText()

####Signature: public function domAppendText($parent, $text)

####Parameters:

* $parent

* $text




####Source Comments:

Add a command to append a text to a DOM element



param string		$parent				The DOM parent element

param string		$text				The HTML text to append



return \Xajax\Plugin\Response



####Writers Description:


####Example:
```
function domAppendTextExample()
{
    $oResponse = new Response()
    $oResponse->domAppendText()
    return $oResponse
}
```