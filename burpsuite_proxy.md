# Setup
1. Install Burp Suite Community Edition
2. Install Chrome
3. Install Firefox

# Usage
1. Turn on the proxy server
2. Direct all the traffic from the system to the burpsuite
3. burpsuite relay the packet to the destination of the target


# Browser Proxy
## Firefox
1. Set the HTTP Proxy "127.0.0.1" Default burpsuite setting
2. Set the Port to "8080" Default burpsuite setting
3. Access the burpsuite CA cert through (http://127.0.0.1:8080), which on the top right corner of the website.
4. Import the CA cert to the Certificate Manager


# System Proxy
## Google Chrome
1. Go to (*Setting* -> *Network & internet* -> *Manual proxy setup*)
2. Turn on *Use a proxy server*
3. Set *Proxy IP address* as 127.0.0.1
4. Set *Port* as 8080
5. Import the CA cert to the *Trusted Root Certification Authorities* (Settings -> Privacy and security -> Advanced -> Manage certificates -> Trusted Root Certification Authorities -> Import...)

# Sometime the application doesn't follow the system Proxy
## (1) Firefox



## (2)  : cURL
#### Default port of the Burp Suite is 8080
(curl -x http://127.0.0.1:8080 https://www.google.com)


## Solution : Transparent Proxy


