## Class: xajax.callback
------------------------------
#### Function: xajax.callback.create

Create a blank callback object.  Two optional arguments let you
set the delay time for the onResponseDelay and onExpiration events.

Returns:

object - The callback object.


##### Signature:xajax.callback.create = function() {
------------------------------
#### Function: xajax.callback.setupTimer

Create a timer to fire an event in the future.  This will
be used fire the onRequestDelay and onExpiration events.

Parameters:

iDelay - (integer):  The amount of time in milliseconds to delay.

Returns:

object - A callback timer object.


##### Signature:xajax.callback.setupTimer = function(iDelay)
------------------------------
#### Function: xajax.callback.clearTimer

Clear a callback timer for the specified function.

Parameters:

oCallback - (object):  The callback object (or objects) that
contain the specified function timer to be cleared.
sFunction - (string):  The name of the function associated
with the timer to be cleared.


##### Signature:xajax.callback.clearTimer = function(oCallback, sFunction)
------------------------------
#### Function: xajax.callback.execute

Execute a callback event.

Parameters:

oCallback - (object):  The callback object (or objects) which
contain the event handlers to be executed.
sFunction - (string):  The name of the event to be triggered.
args - (object):  The request object for this request.


##### Signature:xajax.callback.execute = function(oCallback, sFunction, args) {
