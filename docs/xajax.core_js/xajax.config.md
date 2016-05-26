nada## Class: xajax.config

This class contains all the default configuration settings.  These
are application level settings; however, they can be overridden
by including a xajax.config definition prior to including the
<xajax_core.js> file, or by specifying the appropriate configuration
options on a per call basis.
------------------------------
#### Function: xajax.config.setDefault

This function will set a default configuration option if it is
not already set.

Parameters:
option - (string):
The name of the option that will be set.

defaultValue - (unknown):
The value to use if a value was not already set.


##### Signature:xajax.config.setDefault = function(option, defaultValue) {
