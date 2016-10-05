# The database.php

The database of configuration of each instance is kept in ``application/config/database.php`` in a separate ``db_group``. Since we have assigned the ``db_group`` in our front-controller, we just need to set the same in our ``database.php``.

Here is our ``database.php``:

````php
$active_group = config_item('db_group'); 
$query_builder = TRUE; 

$db['subdomain-1'] = array(
    'dsn'	   => '',
    'hostname' => 'localhost',
    'username' => 'user_1',
    'password' => 'pass_1',
    'database' => 'db_1',
    'dbdriver' => 'mysqli',
    'dbprefix' => '',
    'pconnect' => FALSE,
    'db_debug' => (ENVIRONMENT !== 'production'),
    'cache_on' => FALSE,
    'cachedir' => '',
    'char_set' => 'utf8',
    'dbcollat' => 'utf8_general_ci',
    'swap_pre' => '', 
    'encrypt'  => FALSE, 
    'compress' => FALSE, 
    'stricton' => FALSE, 
    'failover' => array(), 
    'save_queries' => FALSE
); 

$db['subdomain-2'] = array( 
    'dsn'	   => '', 
    'hostname' => 'localhost', 
    'username' => 'user_2', 
    'password' => 'pass_2', 
    'database' => 'db_2', 
    'dbdriver' => 'mysqli', 
    'dbprefix' => '', 
    'pconnect' => FALSE, 
    'db_debug' => (ENVIRONMENT !== 'production'), 
    'cache_on' => FALSE, 
    'cachedir' => '', 
    'char_set' => 'utf8', 
    'dbcollat' => 'utf8_general_ci', 
    'swap_pre' => '', 
    'encrypt' => FALSE, 
    'compress' => FALSE, 
    'stricton' => FALSE, 
    'failover' => array(), 
    'save_queries' => FALSE
);

// ... so on for every instance
````
