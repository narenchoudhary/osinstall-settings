# Proxy Settings

* Define system proxy settings.
    * Go to System Settings > Network > Nerwork Proxy. 
    * Set Method to Manual and add proxy-host and proxy-port.

* Add new network connection.
    * Go to Network Connetions > Add.
    * Select Ethernet and click Create. 
    * Put a connection name. 
    * Go to IPv4 Settings tab.
    * Set Method to Manual.
    * In Addresses section, click on Add.
    * Fill Address, Netmask, and Gateway.
    * Add Additional DNS servers.

* Configure apt-get proxy configuration.
    * `sudo nano /etc/apt/apt.conf`
    * Add username and password to already stated proxy settings. Example:
        
            Acquire::http::proxy "http://username:password@proxyhost:proxyport/";
            Acquire::https::proxy "https://n.choudhary:naren@proxyhost:proxyport/";

* Add `HTTP_PROXY` and `HTTPS_PROXY` env variables in `~/.bashrc`.

        export HTTP_PROXY="http://username:password@proxyhosy:proxyport"
        export HTTPS_PROXY="https://username:password@proxyhosy:proxyport"


