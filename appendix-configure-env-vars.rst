Configure environment variables
*******************************

If you're using the DEB or RPM packages you can change Zammads environment variables by the following commands.

Configure IP
============

::

 zammad config:set ZAMMAD_BIND_IP=0.0.0.0
 systemctl restart zammad


Configure ports
===============

Please note that you also have to reconfigure Nginx when changing the ports!

::

 zammad config:set ZAMMAD_RAILS_PORT=3000
 zammad config:set ZAMMAD_WEBSOCKET_PORT=6042
 systemctl restart zammad
