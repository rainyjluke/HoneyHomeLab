# Setup Kibana site
- Here is the stitch on getting your Kibana site setup.
- First you will need to install docker-compose if you haven't already have it setup on your homelab

sudo apt-get install docker-compose

- It will take a few minutes in order to install. Afterwards go ahead and change directories into the waf_elk site

  cd ~/Honeypot-Project/honeytraps/waf_elk
  cat README.md
- Follow the instructions on the README.md file, you will need to populate an env file for this part. Luckily there is a sample env file found in this directory
- Once you populate the file and changed URL_MISP to the IP MISP will be running on.
  - For our purposes using Kali Linux we will be using the following command

  ifconfig eth0

- Since we are using a Virtual Machine the IP address will look similiar to 10.... of that variety.
- Once that is setup go head and build the docker with the specifications from the README.md
  - This is the part that will use a lot of memory almost 20MB hence why we needed to create a larger space on our Virtual Machines in order to make room for this docker build
  
