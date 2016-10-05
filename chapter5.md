# The constants.php

We just need to add two custom constants in our ``application/config/constants.php`` for our common assets.
```php
    /* 
    |-------------------------------------------------------------------------- 
    | Custom Constants 
    |-------------------------------------------------------------------------- 
    */ 
        defined('ASSETS_BASE') OR define('ASSETS_BASE', 'https://www.example.com/assets/');
        defined('ASSETS_PATH') OR define('ASSETS_PATH', '../assets/'); 
````
The ``ASSETS_BASE`` constant is for our ``stylesheets``, ``javascripts``, ``images``, etc. You will need to prepend all of your asset links (css, js, img, etc) with this constant.

For example:
```html
    <link rel="stylesheet" type="text/css" href="<?=ASSETS_BASE;?>css/styles.css" />
    <img src="<?=ASSETS_BASE;?>images/my-image.jpg" />
````    
The ``ASSETS_PATH`` constant is for our ``php`` scripts to access any files within the ``assets`` folder. Use it for upload paths etc.