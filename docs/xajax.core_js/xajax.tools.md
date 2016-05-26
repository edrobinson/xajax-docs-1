## Class: xajax.tools

This contains utility functions which are used throughout
the xajax core.
------------------------------
#### Function: xajax.tools.$

Shorthand for finding a uniquely named element within
the document.

Parameters:
sId - (string):
The unique name of the element (specified by the
ID attribute), not to be confused with the name
attribute on form elements.

Returns:

object - The element found or null.

Note:
This function uses the <xajax.config.baseDocument>
which allows <xajax> to operate on the main window
document as well as documents from contained
iframes and child windows.

See also:
<xajax.$> and <xjx.$>


##### Signature:xajax.tools.$ = function(sId) {
------------------------------
#### Function: xajax.tools.in_array

Looks for a value within the specified array and, if found,
returns true; otherwise it returns false.

Parameters:
array - (object):
The array to be searched.

valueToCheck - (object):
The value to search for.

Returns:

true : The value is one of the values contained in the
array.

false : The value was not found in the specified array.


##### Signature:xajax.tools.in_array = function(array, valueToCheck) {
------------------------------
#### Function: xajax.tools.doubleQuotes

Replace all occurances of the single quote character with a double
quote character.

Parameters:

haystack - The source string to be scanned.

Returns:  false on error

string - A new string with the modifications applied.


##### Signature:xajax.tools.doubleQuotes = function(haystack) {
------------------------------
#### Function: xajax.tools.singleQuotes

Replace all occurances of the double quote character with a single
quote character.

haystack - The source string to be scanned.

Returns:

string - A new string with the modification applied.


##### Signature:xajax.tools.singleQuotes = function(haystack) {
------------------------------
#### Function: xajax.tools._escape

Determine if the specified value contains special characters and
create a CDATA section so the value can be safely transmitted.

Parameters:

data - (string or other):
The source string value to be evaluated or an object of unknown
type.

Returns:

string - The string value, escaped if necessary or the object provided
if it is not a string.

Note:
When the specified object is NOT a string, the value is returned
as is.


##### Signature:xajax.tools._escape = function(data) {
------------------------------
#### Function: xajax.tools._enforceDataType

Ensure that the javascript variable created is of the correct data type.

Parameters:
value (string)

Returns:

(unknown) - The value provided converted to the correct data type.


##### Signature:xajax.tools._enforceDataType = function(value) {
------------------------------
#### Function: xajax.tools._nodeToObject

Deserialize a javascript object from an XML node.

Parameters:

node - A node, likely from the xml returned by the server.

Returns:

object - The object extracted from the xml node.


##### Signature:xajax.tools._nodeToObject = function(node) {
------------------------------
#### Function: xajax.tools.getRequestObject

Construct an XMLHttpRequest object dependent on the capabilities
of the browser.

Returns:

object - Javascript XHR object.


##### Signature:xajax.tools.getRequestObject = function() {


##### Signature:xajax.tools.getRequestObject = function() {


##### Signature:xajax.tools.getRequestObject = function() {


##### Signature:xajax.tools.getRequestObject = function() {


##### Signature:xajax.tools.getRequestObject = function() {


##### Signature:xajax.tools.getRequestObject = function() {


##### Signature:xajax.tools.getRequestObject = function() {
------------------------------
#### Function: xajax.tools.getBrowserHTML

Insert the specified string of HTML into the document, then
extract it.  This gives the browser the ability to validate
the code and to apply any transformations it deems appropriate.

Parameters:

sValue - (string):
A block of html code or text to be inserted into the
browser's document.

Returns:

The (potentially modified) html code or text.


##### Signature:xajax.tools.getBrowserHTML = function(sValue) {
------------------------------
#### Function: xajax.tools.willChange

Tests to see if the specified data is the same as the current
value of the element's attribute.

Parameters:
element - (string or object):
The element or it's unique name (specified by the ID attribute)

attribute - (string):
The name of the attribute.

newData - (string):
The value to be compared with the current value of the specified
element.

Returns:

true - The specified value differs from the current attribute value.
false - The specified value is the same as the current value.


##### Signature:xajax.tools.willChange = function(element, attribute, newData) {
------------------------------
#### Function: xajax.tools.getFormValues

Build an associative array of form elements and their values from
the specified form.

Parameters:

element - (string): The unique name (id) of the form to be processed.
disabled - (boolean, optional): Include form elements which are currently disabled.
prefix - (string, optional): A prefix used for selecting form elements.

Returns:

An associative array of form element id and value.


##### Signature:xajax.tools.getFormValues = function(parent) {
------------------------------
#### Function: xajax.tools._getFormValues

Used internally by <xajax.tools.getFormValues> to recursively get the value
of form elements.  This function will extract all form element values
regardless of the depth of the element within the form.


##### Signature:xajax.tools._getFormValues = function(aFormValues, children, submitDisabledElements, prefix)
------------------------------
#### Function: xajax.tools._getFormValue

Used internally by <xajax.tools._getFormValues> to extract a single form value.
This will detect the type of element (radio, checkbox, multi-select) and
add it's value(s) to the form values array.

Modified version for multidimensional arrays


##### Signature:xajax.tools._getFormValue = function(aFormValues, child, submitDisabledElements, prefix)
------------------------------
#### Function: xajax.tools.stripOnPrefix

Detect, and if found, remove the prefix 'on' from the specified
string.  This is used while working with event handlers.

Parameters:

sEventName - (string): The string to be modified.

Returns:

string - The modified string.


##### Signature:xajax.tools.stripOnPrefix = function(sEventName) {
------------------------------
#### Function: xajax.tools.addOnPrefix

Detect, and add if not found, the prefix 'on' from the specified
string.  This is used while working with event handlers.

Parameters:

sEventName - (string): The string to be modified.

Returns:

string - The modified string.


##### Signature:xajax.tools.addOnPrefix = function(sEventName) {
