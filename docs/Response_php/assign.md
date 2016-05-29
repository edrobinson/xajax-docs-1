## Response->assign()

####Signature: public function assign($sTarget, $sAttribute, $sData)

####Parameters:

* $sTarget The id of the html element on the browser

* $sAttribute The attribute to be assigned

* $sData The value to be assigned to the attribute

####Source Comments:

Add a command to assign the specified value to the given element's attribute

return \Xajax\Plugin\Response

####Description:
The response assign method is probably the most used method in the class.  
Using assign you can manipulate just about anything of an element in the document.

The element must have a unique Id assigned to it. The name attribute is optional  
but necessary if you want to use the form value retrievel of the xajax javascript.  

This writer makes it a habit to assign both Id and name to document elements. This is  
especially important when dealing with forms and database operations. For example  
if you use db table ield names for both the idand name of the form elements you  
can populat the form from the server with a simple foreach and retrieve the form elements  
by using the xajax.getFormValues() method on the browser.  See the example below...


####Examples:
```
//Populate a form's fields from a db table
function assignExample()
{
    $oResponse = new Response();
    //Read emloyee 12 from the empliyee table into $aFields.
    ...
    foreach($aFields as $key = $val)
    {
        $oResponse->assign($key, 'value', $val); //Assign a value to each field.
    }
    return $oResponse;
}

//Insert text into a div tag
function fillMyDiv()
{
    $text = 'Some Lorum Ipsum text...';
    $oResponse = new Response();
    $oresponse->assign('myDiv','innerHTML',$text); //Note the case of"innerHTML"
    return $oresponse;
}

//Change an element's text color
function recolorForError($id)
{
    $oResponse = new Response();
    $oResponse->assign($id,'style:color','red');
    return $oResponse;
}    
```