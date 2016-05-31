## Class: xajax.responseProcessor
------------------------------
#### Function: xajax.responseProcessor.json

Parse the JSON response into a series of commands.  The commands
are constructed by calling xajax.tools.xml.parseAttributes and
xajax.tools.xml.parseChildren.

Parameters:

oRequest - (object):  The request context object.


##### Signature:xajax.tools.json.processFragment = function(nodes, seq, oRet, oRequest) {


##### Signature:xajax.responseProcessor.json = function (oRequest) {
------------------------------
#### Function: xajax.responseProcessor.xml

Parse the response XML into a series of commands.  The commands
are constructed by calling xajax.tools.xml.parseAttributes and
xajax.tools.xml.parseChildren.

Parameters:

oRequest - (object):  The request context object.


##### Signature:xajax.responseProcessor.xml = function(oRequest) {
