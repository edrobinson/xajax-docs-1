## Response->redirect()

####Signature: public function redirect($sURL, $iDelay=0)

####Parameters:

* $sURL The relative or fully qualified URL

* $iDelay=0 Number of seconds to delay before the redirect occurs 

####Source Comments:
Add a command to ask the browser to navigate to the specified URL.  
return \Xajax\Plugin\Response
####Writers Description:
This method issues a redirect command to the browser. 
Optionally, you can specify a number of seconds to wait.

####Example:
```
function loginCheck()
{
    if (!$this->loggedIn)
    {
        $oResponse = new Response();
        $oResponse->redirect('login.php');
        return $oResponse;
    }
}
```