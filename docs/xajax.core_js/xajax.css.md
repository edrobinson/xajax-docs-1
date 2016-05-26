## Class: xajax.css
------------------------------
#### Function: xajax.css.add

Add a LINK reference to the specified .css file if it does not
already exist in the HEAD of the current document.

Parameters:

filename - (string):  The URI of the .css file to reference.

media - (string):  The media type of the css file (print/screen/handheld,..)

Returns:

true - The operation completed successfully.


##### Signature:xajax.css.add = function(fileName, media) {
------------------------------
#### Function: xajax.css.remove

Locate and remove a LINK reference from the current document's
HEAD.

Parameters:

filename - (string):  The URI of the .css file.

Returns:

true - The operation completed successfully.


##### Signature:xajax.css.remove = function(fileName, media) {
------------------------------
#### Function: xajax.css.waitForCSS

Attempt to detect when all .css files have been loaded once
they are referenced by a LINK tag in the HEAD of the current
document.

Parameters:

args - (object):  The response command object which will contain
the following:

- args.prop - (integer):  The number of 1/10ths of a second
to wait before giving up.

Returns:

true - The .css files appear to be loaded.
false - The .css files do not appear to be loaded and the timeout
has not expired.


##### Signature:xajax.css.waitForCSS = function(args) {
