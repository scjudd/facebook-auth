Facebook-Auth
=============

A simple Facebook OAuth2 authentication backend.

The vast majority of this code was lifted from http://djangosnippets.org/snippets/2065/.

Setup
-----
1.  Add 'facebook-auth' to your INSTALLED\_APPS.
2.  Add 'facebook-auth.auth\_backends.FacebookBackend' to your AUTHENTICATION\_BACKENDS.
3.  Add the following to your settings.py:
    FACEBOOK\_APP\_ID = 'your\_app\_id'  
    FACEBOOK\_API\_KEY = 'your\_api\_key'  
    FACEBOOK\_APP\_SECRET = 'your\_app\_secret'  
    FACEBOOK\_REDIRECT\_URI = 'your\_redirect\_uri'  
    \# http://developers.facebook.com/docs/authentication/permissions/  
    FACEBOOK\_PERMISSIONS = ['email', 'publish\_stream']
4. Run python manage.py syncdb.
