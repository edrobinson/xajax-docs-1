## Class: xajax.tools.queue

This contains the code and variables for building, populating
and processing First In Last Out (FILO) buffers.
------------------------------
#### Function: create

Construct and return a new queue object.

Parameters:

size - (integer):
The number of entries the queue will be able to hold.


##### Signature:xajax.tools.queue.create = function(size) {
------------------------------
#### Function: xajax.tools.queue.retry

Maintains a retry counter for the given object.

Parameters:

obj - (object):
The object to track the retry count for.

count - (integer):
The number of times the operation should be attempted
before a failure is indicated.

Returns:

true - The object has not exhausted all the retries.
false - The object has exhausted the retry count specified.


##### Signature:xajax.tools.queue.retry = function(obj, count) {
------------------------------
#### Function: xajax.tools.queue.rewind

Rewind the buffer head pointer, effectively reinserting the
last retrieved object into the buffer.

Parameters:

theQ - (object):
The queue to be rewound.


##### Signature:xajax.tools.queue.rewind = function(theQ) {
------------------------------
#### Function: xajax.tools.queue.setWakeup

Set or reset a timeout that is used to restart processing
of the queue.  This allows the queue to asynchronously wait
for an event to occur (giving the browser time to process
pending events, like loading files)

Parameters:

theQ - (object):
The queue to process upon timeout.

when - (integer):
The number of milliseconds to wait before starting/
restarting the processing of the queue.


##### Signature:xajax.tools.queue.setWakeup = function(theQ, when) {
------------------------------
#### Function: xajax.tools.queue.process

While entries exist in the queue, pull and entry out and
process it's command.  When a command returns false, the
processing is halted.

Parameters:

theQ - (object): The queue object to process.  This should
have been crated by calling <xajax.tools.queue.create>.

Returns:

true - The queue was fully processed and is now empty.
false - The queue processing was halted before the
queue was fully processed.

Note:

- Use <xajax.tools.queue.setWakeup> or call this function to
cause the queue processing to continue.

- This will clear the associated timeout, this function is not
designed to be reentrant.

- When an exception is caught, do nothing; if the debug module
is installed, it will catch the exception and handle it.


##### Signature:xajax.tools.queue.process = function(theQ) {
------------------------------
#### Function: xajax.tools.queue.push

Push a new object into the tail of the buffer maintained by the
specified queue object.

Parameters:

theQ - (object):
The queue in which you would like the object stored.

obj - (object):
The object you would like stored in the queue.


##### Signature:xajax.tools.queue.push = function(theQ, obj) {
------------------------------
#### Function: xajax.tools.queue.pushFront

Push a new object into the head of the buffer maintained by
the specified queue object.  This effectively pushes an object
to the front of the queue... it will be processed first.

Parameters:

theQ - (object):
The queue in which you would like the object stored.

obj - (object):
The object you would like stored in the queue.


##### Signature:xajax.tools.queue.pushFront = function(theQ, obj) {
------------------------------
#### Function: xajax.tools.queue.pop

Attempt to pop an object off the head of the queue.

Parameters:

theQ - (object):
The queue object you would like to modify.

Returns:

object - The object that was at the head of the queue or
null if the queue was empty.


##### Signature:xajax.tools.queue.pop = function(theQ) {
