## Class: xajax.js

Contains the functions for javascript file and function
manipulation.
------------------------------
#### Function: xajax.js.includeScriptOnce

Add a reference to the specified script file if one does not
already exist in the HEAD of the current document.

This will effecitvely cause the script file to be loaded in
the browser.

Parameters:

fileName - (string):  The URI of the file.

Returns:

true - The reference exists or was added.


##### Signature:xajax.js.includeScriptOnce = function(command) {
------------------------------
#### Function: xajax.js.includeScript

Adds a SCRIPT tag referencing the specified file.  This
effectively causes the script to be loaded in the browser.

Parameters:

command (object) - Xajax response object

Returns:

true - The reference was added.


##### Signature:xajax.js.includeScript = function(command) {
------------------------------
#### Function: xajax.js.removeScript

Locates a SCRIPT tag in the HEAD of the document which references
the specified file and removes it.

Parameters:

command (object) - Xajax response object

Returns:

true - The script was not found or was removed.


##### Signature:xajax.js.removeScript = function(command) {
------------------------------
#### Function: xajax.js.sleep

Causes the processing of items in the queue to be delayed
for the specified amount of time.  This is an asynchronous
operation, therefore, other operations will be given an
opportunity to execute during this delay.

Parameters:

args - (object):  The response command containing the following
parameters.
- args.prop: The number of 10ths of a second to sleep.

Returns:

true - The sleep operation completed.
false - The sleep time has not yet expired, continue sleeping.


##### Signature:xajax.js.sleep = function(command) {
------------------------------
#### Function: xajax.js.confirmCommands

Prompt the user with the specified text, if the user responds by clicking
cancel, then skip the specified number of commands in the response command
queue.  If the user clicks Ok, the command processing resumes normal
operation.

Parameters:

command (object) - xajax response object

Returns:

true - The operation completed successfully.


##### Signature:xajax.js.confirmCommands = function(command) {
------------------------------
#### Function: xajax.js.execute

Execute the specified string of javascript code, using the current
script context.

Parameters:

args - The response command object containing the following:
- args.data: (string):  The javascript to be evaluated.
- args.context: (object):  The javascript object that to be
referenced as 'this' in the script.

Returns:

unknown - A value set by the script using 'returnValue = '
true - If the script does not set a returnValue.


##### Signature:xajax.js.execute = function(args) {


##### Signature:args.context.xajaxDelegateCall = function() {
------------------------------
#### Function: xajax.js.waitFor

Test for the specified condition, using the current script
context; if the result is false, sleep for 1/10th of a
second and try again.

Parameters:

args - The response command object containing the following:

- args.data: (string):  The javascript to evaluate.
- args.prop: (integer):  The number of 1/10ths of a
second to wait before giving up.
- args.context: (object):  The current script context object
which is accessable in the javascript being evaulated
via the 'this' keyword.

Returns:

false - The condition evaulates to false and the sleep time
has not expired.
true - The condition evaluates to true or the sleep time has
expired.


##### Signature:xajax.js.waitFor = function(args) {


##### Signature:args.context.xajaxDelegateCall = function() {
------------------------------
#### Function: xajax.js.call

Call a javascript function with a series of parameters using
the current script context.

Parameters:

args - The response command object containing the following:
- args.data: (array):  The parameters to pass to the function.
- args.func: (string):  The name of the function to call.
- args.context: (object):  The current script context object
which is accessable in the function name via the 'this'
keyword.

Returns:

true - The call completed successfully.


##### Signature:xajax.js.call = function(args) {


##### Signature:args.context.xajaxDelegateCall = function() {
------------------------------
#### Function: xajax.js.setFunction

Constructs the specified function using the specified javascript
as the body of the function.

Parameters:

args - The response command object which contains the following:

- args.func: (string):  The name of the function to construct.
- args.data: (string):  The script that will be the function body.
- args.context: (object):  The current script context object
which is accessable in the script name via the 'this' keyword.

Returns:

true - The function was constructed successfully.


##### Signature:xajax.js.setFunction = function(args) {


##### Signature:code.push(' = function(');


##### Signature:args.context.xajaxDelegateCall = function() {
------------------------------
#### Function: xajax.js.wrapFunction

Construct a javascript function which will call the original function with
the same name, potentially executing code before and after the call to the
original function.

Parameters:

args - (object):  The response command object which will contain
the following:

- args.func: (string):  The name of the function to be wrapped.
- args.prop: (string):  List of parameters used when calling the function.
- args.data: (array):  The portions of code to be called before, after
or even between calls to the original function.
- args.context: (object):  The current script context object which is
accessable in the function name and body via the 'this' keyword.

Returns:

true - The wrapper function was constructed successfully.


##### Signature:xajax.js.wrapFunction = function(args) {


##### Signature:args.context.xajaxDelegateCall = function() {
------------------------------
#### Function: xajax.js.makeWrapper


Helper function used in the wrapping of an existing javascript function.

Parameters:

origFun - (string):  The name of the original function.
args - (string):  The list of parameters used when calling the function.
codeBlocks - (array):  Array of strings of javascript code to be executed
before, after and perhaps between calls to the original function.
returnVariable - (string):  The name of the variable used to retain the
return value from the call to the original function.
context - (object):  The current script context object which is accessable
in the function name and body via the 'this' keyword.

Returns:

object - The complete wrapper function.


##### Signature:xajax.js.makeWrapper = function(origFun, args, codeBlocks, returnVariable, context) {


##### Signature:var code = 'wrapper = function(';


##### Signature:context.xajaxDelegateCall = function() {
