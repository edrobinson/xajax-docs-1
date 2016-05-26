## Class: xajax.dom
------------------------------
#### Function: xajax.dom.assign

Assign an element's attribute to the specified value.

Parameters:

element - (object):  The HTML element to effect.
property - (string):  The name of the attribute to set.
data - (string):  The new value to be applied.

Returns:

true - The operation completed successfully.


##### Signature:xajax.dom.assign = function(element, property, data) {
------------------------------
#### Function: xajax.dom.append

Append the specified value to an element's attribute.

Parameters:

element - (object):  The HTML element to effect.
property - (string):  The name of the attribute to append to.
data - (string):  The new value to be appended.

Returns:

true - The operation completed successfully.


##### Signature:xajax.dom.append = function(element, property, data) {
------------------------------
#### Function: xajax.dom.prepend

Prepend the specified value to an element's attribute.

Parameters:

element - (object):  The HTML element to effect.
property - (string):  The name of the attribute.
data - (string):  The new value to be prepended.

Returns:

true - The operation completed successfully.


##### Signature:xajax.dom.prepend = function(element, property, data) {
------------------------------
#### Function: xajax.dom.replace

Search and replace the specified text.

Parameters:

element - (string or object):  The name of, or the element itself which is
to be modified.
sAttribute - (string):  The name of the attribute to be set.
aData - (array):  The search text and replacement text.

Returns:

true - The operation completed successfully.


##### Signature:xajax.dom.replace = function(element, sAttribute, aData) {
------------------------------
#### Function: xajax.dom.remove

Delete an element.

Parameters:

element - (string or object):  The name of, or the element itself which
will be deleted.

Returns:

true - The operation completed successfully.


##### Signature:xajax.dom.remove = function(element) {
------------------------------
#### Function: xajax.dom.create

Create a new element and append it to the specified parent element.

Parameters:

objParent - (string or object):  The name of, or the element itself
which will contain the new element.
sTag - (string):  The tag name for the new element.
sId - (string):  The value to be assigned to the id attribute of
the new element.

Returns:

true - The operation completed successfully.


##### Signature:xajax.dom.create = function(objParent, sTag, sId) {
------------------------------
#### Function: xajax.dom.insert

Insert a new element before the specified element.

Parameters:

objSibling - (string or object):  The name of, or the element itself
that will be used as the reference point for insertion.
sTag - (string):  The tag name for the new element.
sId - (string):  The value that will be assigned to the new element's
id attribute.

Returns:

true - The operation completed successfully.


##### Signature:xajax.dom.insert = function(objSibling, sTag, sId) {
------------------------------
#### Function: xajax.dom.insertAfter

Insert a new element after the specified element.

Parameters:

objSibling - (string or object):  The name of, or the element itself
that will be used as the reference point for insertion.
sTag - (string):  The tag name for the new element.
sId - (string):  The value that will be assigned to the new element's
id attribute.

Returns:

true - The operation completed successfully.


##### Signature:xajax.dom.insertAfter = function(objSibling, sTag, sId) {
------------------------------
#### Function: xajax.dom.contextAssign

Assign a value to a named member of the current script context object.

Parameters:

args - (object):  The response command object which will contain the
following:

- args.prop: (string):  The name of the member to assign.
- args.data: (string or object):  The value to assign to the member.
- args.context: (object):  The current script context object which
is accessable via the 'this' keyword.

Returns:

true - The operation completed successfully.


##### Signature:xajax.dom.contextAssign = function(args) {


##### Signature:args.context.xajaxDelegateCall = function(data) {
------------------------------
#### Function: xajax.dom.contextAppend

Appends a value to a named member of the current script context object.

Parameters:

args - (object):  The response command object which will contain the
following:

- args.prop: (string):  The name of the member to append to.
- args.data: (string or object):  The value to append to the member.
- args.context: (object):  The current script context object which
is accessable via the 'this' keyword.

Returns:

true - The operation completed successfully.


##### Signature:xajax.dom.contextAppend = function(args) {


##### Signature:args.context.xajaxDelegateCall = function(data) {
------------------------------
#### Function: xajax.dom.contextPrepend

Prepend a value to a named member of the current script context object.

Parameters:

args - (object):  The response command object which will contain the
following:

- args.prop: (string):  The name of the member to prepend to.
- args.data: (string or object):  The value to prepend to the member.
- args.context: (object):  The current script context object which
is accessable via the 'this' keyword.

Returns:

true - The operation completed successfully.


##### Signature:xajax.dom.contextPrepend = function(args) {


##### Signature:args.context.xajaxDelegateCall = function(data) {
