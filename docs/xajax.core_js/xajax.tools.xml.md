## Class: xajax.tools.xml

An object that contains utility function for processing
xml response packets.
------------------------------
#### Function: xajax.tools.xml.parseAttributes

Take the parameters passed in the command of the XML response
and convert them to parameters of the args object.  This will
serve as the command object which will be stored in the
response command queue.

Parameters:

child - (object):  The xml child node which contains the
attributes for the current response command.

obj - (object):  The current response command that will have the
attributes applied.


##### Signature:xajax.tools.xml.parseAttributes = function(child, obj) {
------------------------------
#### Function: xajax.tools.xml.parseChildren

Parses the child nodes of the command of the response XML.  Generally,
the child nodes contain the data element of the command; this member
may be an object, which will be deserialized by xajax._nodeToObject

Parameters:

child - (object):   The xml node that contains the child (data) for
the current response command object.

obj - (object):  The response command object.


##### Signature:xajax.tools.xml.parseChildren = function(child, obj) {
------------------------------
#### Function: xajax.tools.xml.processFragment

Parameters:

xmlNode - (object):  The first xml node in the xml fragment.
seq - (number):  A counter used to keep track of the sequence
of this command in the response.
oRet - (object):  A variable that is used to return the request
"return value" for use with synchronous requests.


##### Signature:xajax.tools.xml.processFragment = function(xmlNode, seq, oRet, oRequest) {
