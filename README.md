undercake
=========

This is a small adaptation of Underscore.php v1.3.1 for CakePHP.

As __() is already used by CakePHP for internationalization, the class, function and internal variables were changed to _uc, _uc(), $_uc.

This is my only contribution so far, but it gets the job done!

I will try to make a component out of this at a later time.

USAGE EX: ```_uc( $myVar )->map(function($n) { return $n * 2; });```

Note: The ```__::map($myVar, function($n) { return $n * 2; }); ``` method does not work.

For extended documentation, see the Underscore.php page at
http://brianhaveri.github.io/Underscore.php

#To use in CakePHP

1. Copy undercake.php to your app/vendors folder
2. Include ```App::import('Vendor', 'undercake');``` right before ```class AppController extends Controller {``` in your app_controller.php file
3. Use the marvels of Underscore.php like this: ```_uc( $myVar )->map(function($n) { return $n * 2; });```
