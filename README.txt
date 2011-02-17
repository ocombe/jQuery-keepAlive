jQuery keepAlive plugin
https://github.com/Aldri/jQuery-keepAlive

Copyright 2011, Olivier Combe
Dual licensed under the MIT or GPL Version 2 licenses.
http://jquery.org/license

Version 1.0 2011-02-17

* Description :
This plugin does a simple ajax call to an url every x minutes (10 minutes by default).
The goal is to force the server to refresh the user's session timeout in order to keep it alive for as long as the user is on your web site.

* Usage :
Add the js file (jquery.keepAlive.js or jquery.keepAlive.min.js) and the php file (keepAlive.php) in your folder.
Include the js file in your page and call the function :
$.fn.keepAlive();

* Options :
You can set the url of your php file :
$.fn.keepAlive({url: 'somefolder/keepAlive.php'});

You can set the timer of the ajax calls :
$.fn.keepAlive({timer: 5000}); // call every 5 seconds

Or you can set both :
$.fn.keepAlive({url: 'somefolder/keepAlive.php', timer: 5000}); // call every 5 seconds

If you want to stop the ajax calls for some reason just call :
$.fn.keepAlive('stop');