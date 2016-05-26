## Class: xajax.config.status

Provides support for updating the browser's status bar during
the request process.  By splitting the status bar functionality
into an object, the xajax developer has the opportunity to
customize the status bar messages prior to sending xajax requests.
------------------------------
#### Function: update

Constructs and returns a set of event handlers that will be
called by the xajax framework to set the status bar messages.
------------------------------
#### Function: dontUpdate

Constructs and returns a set of event handlers that will be
called by the xajax framework where status bar updates
would normally occur.
