# Apache httpd.conf directory settings

If you run into access problems in Apache, getting a message like ```You don't have permission to access this resource.```,
try changing the directory settings in http.conf

I ran into this problem after updating to MacOS Catalina.


```bash
<Directory />
    #Options FollowSymLinks
    Options Indexes FollowSymLinks Includes ExecCGI
    AllowOverride All
    Order deny,allow
    Allow from all
</Directory>
```

[More about this here](https://stackoverflow.com/questions/10873295/error-message-forbidden-you-dont-have-permission-to-access-on-this-server)
