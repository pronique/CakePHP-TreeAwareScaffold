# TreeAwareScaffold Plugin for CakePHP 2 #

This CakePHP plugin overrides the builtin scaffolding in CakePHP.  The plugin hides the lft,rght fields in all scaffold views for TreeBehavior Models.  It also generates ordered/indented dropdowns on forms when the belongsTo model implements TreeBehavior.

The TreeAwareScaffold plugin was created as part of a [CakePHP tutorial found here](http://www.pronique.com/blog/how-to-create-your-own-scaffolding-plugin-for-cakephp2) to demonstrate how to replace the builtin CakePHP Scaffolding.

## Installation ##

    sudo git clone https://github.com/pronique/CakePHP-TreeAwareScaffold app/Plugin/TreeAwareScaffold
    
    //Enable plugin in app/Config/bootstrap.php
    CakePlugin::load('TreeAwareScaffold');
    
    
## Example Usage  ##

Add the following to the top of AppController.php
```php
App::uses('Scaffold', 'TreeAwareScaffold.Controller');

App::uses('ScaffoldView', 'TreeAwareScaffold.View');
``` 

That's it!!!!  All other scaffolding functionality remains the same.

## Requirements ##

* PHP version: PHP 5.2+
* CakePHP version: 2.0+

## License ##

Copyright 2011-2012, [PRONIQUE Software](http://pronique.com)

Licensed under [The MIT License](http://www.opensource.org/licenses/mit-license.php)<br/>
Redistributions of files must retain the above copyright notice.

--------------------------------------------------------------------------
The TreeAwareBehavior plugin for CakePHP is Open Source Software created and managed by PRONIQUE Software.

http://www.pronique.com
