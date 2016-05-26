## Class: xajax.events
------------------------------
#### Function: xajax.events.setEvent

Set an event handler.

Parameters:

command - (object): Response command object.
- id: Element ID
- prop: Event
- data: Code

Returns:

true - The operation completed successfully.


##### Signature:xajax.events.setEvent = function(command) {


##### Signature:eval('element.' + sEvent + ' = function(e) { ' + code + '; }');
------------------------------
#### Function: xajax.events.addHandler

Add an event handler to the specified element.

Parameters:

element - (string or object):  The name of, or the element itself
which will have the event handler assigned.
sEvent - (string):  The name of the event.
fun - (string):  The function to be called.

Returns:

true - The operation completed successfully.


##### Signature:xajax.events.addHandler = function(element, sEvent, fun) {


##### Signature:xajax.events.addHandler = function(command) {


##### Signature:xajax.events.addHandler = function(command) {
------------------------------
#### Function: xajax.events.removeHandler

Remove an event handler from an element.

Parameters:

element - (string or object):  The name of, or the element itself which
will have the event handler removed.
event - (string):  The name of the event for which this handler is
associated.
fun - The function to be removed.

Returns:

true - The operation completed successfully.


##### Signature:xajax.events.removeHandler = function(element, sEvent, fun) {


##### Signature:xajax.events.removeHandler = function(command) {


##### Signature:xajax.events.removeHandler = function(command) {
