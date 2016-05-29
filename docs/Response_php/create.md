## Response->create()

####Signature: public function create($sParent, $sTag, $sId)

####Parameters:

* $sParent The id of the parent element

* $sTag The tag name to be used for the new element

* $sId The id to assign to the new element
* return \Xajax\Plugin\Response

####Source Comments:

Add a command to create a new element on the browser.

####Writers Description:
Use create to add a new element to the html page.
The parent element is expressed as its id attribute.
The tag is specified as div, input, etc.
The final parameter is the id of the new element. It should be unique on the page.

####Example:
```
function createExample()
{
    $oResponse = new Response()
    $oResponse->create('parentId','div','newdivId');
    return $oResponse
}
```