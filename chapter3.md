# The index.php

The index.php is our front-controller for each application instance.

Here are the things to change:

### The system path
````php
    /*  
     *--------------------------  
     * SYSTEM DIRECTORY NAME  
     *--------------------------  
     *  
     * This variable must contain the name of your "system" directory.  
     * Set the path if it is not in the same directory as this file.  
     */
             $system_path = '../../system'; 
    
````  
  
  
### The application path
````php
    /*  
     *-------------------------------  
     * APPLICATION DIRECTORY NAME 
     *-------------------------------  
     * 
     * If you want this front controller to use a different "application"  
     * directory than the default one you can set its name here. The directory  
     * can also be renamed or relocated anywhere on your server. If you do,  
     * use an absolute (full) server path.  
     * For more info please see the user guide:  
     *  
     *  https://codeigniter.com/user_guide/general/managing_apps.html  
     *  
     *  NO TRAILING SLASH!  
     */
             $application_folder = '../../application';
````   
  
  
### Custom CONFIG
````php
    /*  
     *--------------------------  
     *  CUSTOM CONFIG VALUES  
     *--------------------------  
     * 
     * The $assign_to_config array below will be passed dynamically to the  
     * config class when initialized. This allows you to set custom config  
     * items or override any default config values found in the config.php file.  
     * This can be handy as it permits you to share one application between  
     * multiple front controller files, with each file containing different  
     * config values.  
     *   
     * Un-comment the $assign_to_config array below to use this feature  
     */ 	
             $assign_to_config['base_url'] = 'http://sub-domain-n.example.com'; 
             
             // your database group (see next chapter)
             $assign_to_config['db_group'] = 'subdomain-n';  
             $assign_to_config['encryption_key'] = 'my123secret456encryption789key'; 
             $assign_to_config['cookie_domain'] = '.sub-domain-n.example.com';
````