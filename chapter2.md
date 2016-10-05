# The .htaccess

Here's the code for our ``.htaccess``:

    # Disable directory listing
    Options All -Indexes 
    
    # Domain filter
    RewriteEngine on 
    RewriteCond %{HTTP_HOST} !^sub-domain-n\.example\.com$ [NC] 
    RewriteRule ^ - [F] 
    
    # Remove index.php from URLs
    RewriteCond $1 !^(index\.php|assets|robots\.txt) 
    RewriteRule ^(.*)$ index.php/$1 [L]


The first rule - the domain filter - blocks all traffic except for the specified sub domain.
The second rule removes the ``index.php`` from our URLs.

