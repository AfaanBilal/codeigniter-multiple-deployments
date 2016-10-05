# The directory structure

The directory structure of our application will be somewhat as follows:

    application
    system
    public_html
      assets
      sub-domain-1.example.com
      sub-domain-2.example.com
      sub-domain-3.example.com
      ...
      sub-domain-n.example.com

In the above structure, ``application`` is our application directory, ``system`` contains the CodeIgniter system files and ``public_html`` will be the *document root* of our domain ``example.com``. We have an ``assets`` directory inside our document root which will hold the common assets for our application instances. 