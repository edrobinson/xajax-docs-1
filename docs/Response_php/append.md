## Response->append()

####Signature: public function append($sTarget, $sAttribute, $sData)

####Parameters:

* $sTarget

* $sAttribute

* $sData

####Source Comments:

Add a command to append the specified data to the given element's attribute

param string		$sTarget			The id of the element to be updated

param string		$sAttribute			The name of the attribute to be appended to

param string		$sData				The data to be appended to the attribute

return \Xajax\Plugin\Response

####Description:
Use this method to add to the end of an element.

####Example:
    //This example from the Xajax forum adds divs to a form,
    //inserts an input in the new divs and populates them.
    function addFields() {
		$objResponse=new Response();
			
		$objResponse->append( 'myform', "innerHTML", '<div id="mydiv1"></div>' ); //add a div   
		$objResponse->createInput("mydiv1", "text", "field[]", "id1" ); //insert an input into it
		$objResponse->append( 'myform', "innerHTML", '<div id="mydiv2"></div>' ); //add another div
		$objResponse->createInput("mydiv2", "text", "field[]", "id2" ); //and insert another input 
		$objResponse->assign( "id1", "value", "val1" ); //Populate the new inputs
		$objResponse->assign( "id2", "value", "val2" );
		return $objResponse;
    }
