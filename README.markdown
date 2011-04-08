Description
===========

A way to run multiple instances of apache/php on the same box, on different ports, as different users with a minimum of configuration.
If you are set up as I am (with apache in /usr/local/apache2) your properly written app with all other dependencies resolved *should* 
just run after following the usage instructions below. 


Usage
=====

Assuming you are on a Fedora 8 server and have compiled and installed the latest apache2 and php from tarball
This setup is known to work with Wordpress.

1. clone to a directory
2. go there
3. put your php app in htdocs/
2. set the port in your environment
    $ export SRVPORT=2222 # or the port of your choice
3. set the location of httpd in your environment
    $ export APACHEBIN=/usr/local/apache2/bin/httpd
3. cd to your dir
4. bin/run_apache to start your server 
5. bin/stop_apache to stop your server
