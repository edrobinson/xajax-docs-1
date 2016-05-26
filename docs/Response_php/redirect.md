## Response->redirect()

####Signature: public function redirect($sURL, $iDelay=0)

####Parameters:

* $sURL

* $iDelay=0




####Source Comments:

Add a command to ask the browser to navigate to the specified URL



param string		$sURL				The relative or fully qualified URL

param integer		$iDelay				Number of seconds to delay before the redirect occurs



return \Xajax\Plugin\Response



####Description:


####Example:
<code><pre>
function redirectExample()
{
    $oResponse = new Response()
    $oResponse->redirect()
    return $oResponse
}
</pre></code>