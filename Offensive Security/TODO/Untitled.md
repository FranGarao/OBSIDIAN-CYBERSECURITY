On opening Firefox and putting http://[target ip] , the browser returns a message about being unable
to find that site. Looking in the URL bar, it now shows http://unika.htb . The website has redirected the
browser to a new URL, and your host doesn't know how to find unika.htb . This webserver is employing
name-based Virtual Hosting for serving the requests.
Name-Based Virtual hosting is a method for hosting multiple domain names (with separate handling of
each name) on a single server. This allows one server to share its resources, such as memory and processor
cycles, without requiring all the services to be used by the same hostname.
The web server checks the domain name provided in the Host header field of the HTTP request and sends
a response according to that.
The /etc/hosts file is used to resolve a hostname into an IP address & thus we will need to add an entry in
the /etc/hosts file for this domain to enable the browser to resolve the address for unika.htb

echo "10.129.128.223 unika.htb" | sudo tee -a /etc/hosts