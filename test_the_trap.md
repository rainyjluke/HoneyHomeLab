# Testing the Trap

After setting up all three repositiories as specified in their specific README.md, we can now test the trap out. So we'll generate some traffic.

curl 'localhost:9091/index.html?exec=/bin/bash'
curl 'http://localhost:9091/?q="><script>alert(1)</script>'

- It will take a little bit of sometime in order to for the traffic to be recorded on your misp and kibana sites. But it should populate on those sites after a minute or so

To be clear there is a lot more informaiton on OWASP Honeypot site https://github.com/OWASP/Honeypot-Project
More information and more in depth explanation of the OWASP honeypot is all right there. 
Happy Trapping
