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
     * ...  
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
     * ... 
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
     * ... 
     */ 	
             $assign_to_config['base_url'] = 'http://sub-domain-n.example.com'; 
             
             // your database group (see next chapter)
             $assign_to_config['db_group'] = 'subdomain-n';  
             $assign_to_config['encryption_key'] = 'my123secret456encryption789key'; 
             $assign_to_config['cookie_domain'] = '.sub-domain-n.example.com';
````
