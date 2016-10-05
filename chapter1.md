# The Directory Structure
The directory structure of our application will be somewhat as follows:
````
application/
system/
public_html/
  assets/
  sub-domain-1.example.com/
    assets/
    .htaccess
    index.php
  sub-domain-2.example.com/
    assets/
    .htaccess
    index.php
  sub-domain-3.example.com/
    assets/
    .htaccess
    index.php
  ...
  sub-domain-n.example.com/
    assets/
    .htaccess
    index.php
````
In the above structure: 
- ``application`` is our application directory
- ``system`` contains the CodeIgniter system files, and 
- ``public_html`` will be the *document root* of our domain ``example.com``. 
- ``assets`` directory inside our document root will hold the common assets for our application instances. 
- ``sub-domain-1.example.com`` through ``sub-domain-n.example.com`` will hold our front controllers for each instance of our application. Set the document roots of the sub domains to these directories.
- ``assets`` directory inside each of the ``sub-domain-n.example.com`` will hold any instance specific assets that we may need (Optional).
- ``.htaccess`` inside our each of the ``sub-domain-n.example`` will help us remove the ``index.php`` from our URLs as well as implement a domain filter.

Now, we'll walk through the files that need to be modified one-by-one.