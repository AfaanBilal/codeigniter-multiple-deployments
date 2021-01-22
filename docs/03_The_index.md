# The index.php

The ``index.php`` is our front-controller for each application instance.
Here are the things to change:  
### The system path
````php
 $system_path = '../../system'; 
````  
### The application path
````php
 $application_folder = '../../application';
````   
### Custom CONFIG
````php	
 $assign_to_config['base_url'] = 'https://sub-domain-n.example.com'; 
 // your database group (see next chapter)  
 $assign_to_config['db_group'] = 'subdomain-n';  
 $assign_to_config['encryption_key'] = 'my123secret456key'; 
 $assign_to_config['cookie_domain'] = '.sub-domain-n.example.com';
````
