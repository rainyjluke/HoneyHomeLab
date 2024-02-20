# Modsec Setup
- After setting up both misp and waf_elk you'll want to finish the honeypot by following these steps.
- First off you'll want to change directories and get into waf_modsec.

cd ~/Honeypot-Project/honeytraps/waf_modsec

- After opening up this directory, you'll want to copy the env file that is there and add the IP address that the env file is running on. This should be the same IP address
  you're Virtual Machine is running on
    - You can check to see what your IP address with this command

  ifconfig eth0

- To copy the env file you want to do this command

cp sample-env 
docker-compose build

- You'll build the docker containter once more this will fill up more space on your VM. Doing these docker containers will fill up space but that is why we set up our VMS to 50MB
- To get the docker container started follow this command

docker-compose up

- You might need sudo privileges in order to run it, but once its up you'll be set for your honeypot!
- By design the ports open will be 9091, 8080, 8000, 8888. 
