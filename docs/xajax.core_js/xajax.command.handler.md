## Class: xajax.command.handler

The object that manages command handlers.
------------------------------
#### Function: xajax.command.handler.register

Registers a new command handler.


##### Signature:xajax.command.handler.register = function(shortName, func) {
------------------------------
#### Function: xajax.command.handler.unregister

Unregisters and returns a command handler.

Parameters:
shortName - (string): The name of the command handler.

Returns:
func - (function): The unregistered function.


##### Signature:xajax.command.handler.unregister = function(shortName) {
------------------------------
#### Function: xajax.command.handler.isRegistered


Parameters:
command - (object):
- cmd: The Name of the function.

Returns:

boolean - (true or false): depending on whether a command handler has
been created for the specified command (object).



##### Signature:xajax.command.handler.isRegistered = function(command) {
------------------------------
#### Function: xajax.command.handler.call

Calls the registered command handler for the specified command
(you should always check isRegistered before calling this function)

Parameters:
command - (object):
- cmd: The Name of the function.

Returns:
true - (boolean) :


##### Signature:xajax.command.handler.call = function(command) {
------------------------------
#### Function: xajax.initializeRequest

Initialize a request object, populating default settings, where
call specific settings are not already provided.

Parameters:

oRequest - (object):  An object that specifies call specific settings
that will, in addition, be used to store all request related
values.  This includes temporary values used internally by xajax.


##### Signature:xajax.initializeRequest = function(oRequest) {


##### Signature:oRequest.append = function(opt, def) {


##### Signature:oRequest.set = function(option, defaultValue) {


##### Signature:lcb.take = function(frm, opt) {
------------------------------
#### Function: xajax.processParameters

Processes request specific parameters and generates the temporary
variables needed by xajax to initiate and process the request.

Parameters:

oRequest - A request object, created initially by a call to
<xajax.initializeRequest>

Note:
This is called once per request; upon a request failure, this
will not be called for additional retries.


##### Signature:xajax.processParameters = function(oRequest) {
------------------------------
#### Function: xajax.prepareRequest

Prepares the XMLHttpRequest object for this xajax request.

Parameters:

oRequest - (object):  An object created by a call to <xajax.initializeRequest>
which already contains the necessary parameters and temporary variables
needed to initiate and process a xajax request.

Note:
This is called each time a request object is being prepared for a
call to the server.  If the request is retried, the request must be
prepared again.


##### Signature:xajax.prepareRequest = function(oRequest) {


##### Signature:oRequest.setRequestHeaders = function(headers) {


##### Signature:oRequest.setCommonRequestHeaders = function() {


##### Signature:oRequest.setPostRequestHeaders = function() {


##### Signature:oRequest.setGetRequestHeaders = function() {


##### Signature:oRequest.request.onreadystatechange = function() {


##### Signature:oRequest.finishRequest = function() {


##### Signature:oRequest.finishRequest = function() {


##### Signature:oRequest.open = function() {


##### Signature:oRequest.open = function() {


##### Signature:oRequest.applyRequestHeaders = function() {


##### Signature:oRequest.applyRequestHeaders = function() {
------------------------------
#### Function: xajax.request

Initiates a request to the server.

Parameters:

functionName - (object):  An object containing the name of the function to execute
on the server. The standard request is: {xjxfun:'function_name'}

oRequest - (object, optional):  A request object which
may contain call specific parameters.  This object will be
used by xajax to store all the request parameters as well
as temporary variables needed during the processing of the
request.



##### Signature:xajax.request = function() {
------------------------------
#### Function: xajax.submitRequest

Create a request object and submit the request using the specified
request type; all request parameters should be finalized by this
point.  Upon failure of a POST, this function will fall back to a
GET request.

Parameters:

oRequest - (object):  The request context object.


##### Signature:xajax.submitRequest = function(oRequest) {
------------------------------
#### Function: xajax._internalSend

This function is used internally by xajax to initiate a request to the
server.

Parameters:

oRequest - (object):  The request context object.


##### Signature:xajax._internalSend = function(oRequest) {
------------------------------
#### Function: xajax.abortRequest

Abort the request.

Parameters:

oRequest - (object):  The request context object.


##### Signature:xajax.abortRequest = function(oRequest)
------------------------------
#### Function: xajax.responseReceived

Process the response.

Parameters:

oRequest - (object):  The request context object.


##### Signature:xajax.responseReceived = function(oRequest) {
------------------------------
#### Function: xajax.getResponseProcessor

This function attempts to determine, based on the content type of the
reponse, what processor should be used for handling the response data.

The default xajax response will be text/xml which will invoke the
xajax xml response processor.  Other response processors may be added
in the future.  The user can specify their own response processor on
a call by call basis.

Parameters:

oRequest - (object):  The request context object.


##### Signature:xajax.getResponseProcessor = function(oRequest) {
------------------------------
#### Function: xajax.executeCommand

Perform a lookup on the command specified by the response command
object passed in the first parameter.  If the command exists, the
function checks to see if the command references a DOM object by
ID; if so, the object is located within the DOM and added to the
command data.  The command handler is then called.

If the command handler returns true, it is assumed that the command
completed successfully.  If the command handler returns false, then the
command is considered pending; xajax enters a wait state.  It is up
to the command handler to set an interval, timeout or event handler
which will restart the xajax response processing.

Parameters:

obj - (object):  The response command to be executed.

Returns:

true - The command completed successfully.
false - The command signalled that it needs to pause processing.


##### Signature:xajax.executeCommand = function(command) {
------------------------------
#### Function: xajax.completeResponse

Called by the response command queue processor when all commands have
been processed.

Parameters:

oRequest - (object):  The request context object.


##### Signature:xajax.completeResponse = function(oRequest) {
------------------------------
#### Function: xajax.$

Shortcut to <xajax.tools.$>.
------------------------------
#### Function: xajax.getFormValues

Shortcut to <xajax.tools.getFormValues>.
