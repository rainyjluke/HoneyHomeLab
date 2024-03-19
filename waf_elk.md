# Setup Kibana site
- Listed below is how you will set up waf_elk.md. It is preferrable that you set up misp before waf_elk.

- First you will need to install docker-compose if you haven't already have it setup on your homelab.

sudo apt-get install docker-compose

- It will take a few minutes in order to install. Afterwards go ahead and change directories into the waf_elk site.

  cd ~/Honeypot-Project/honeytraps/waf_elk
  cat README.md
- Follow the instructions on the README.md file, you will need to populate an env file for this part. Luckily there is a sample env file found in this directory.
- Once you populate the file and changed URL_MISP to the IP MISP will be running on.
  - For our purposes using Kali Linux we will be using the following command

  ifconfig eth0

![image](https://github.com/rainyjluke/HoneyHomeLab/assets/119358099/e5ba936a-809b-4022-bd6a-afa1a6b5f1f6)

- Most virtual machines will show the IP address of a variety of 10.....
- Afterwards you'll change the MISP_KEY found on the site your created from the misp site
- Once that is setup go head and build the docker with the specifications from the README.md
  - It is this part that it will consue 20 MB hence the need for at least 50 MB for the VM.
- The you'll start the build for docker and start the containers with these commands:

sudo docker-compose build
./start_docker.sh

- It might take a a minute in order to build the docker container and start it. When finished, it will continue running as the site is open for your IP address.
- You'll want to open the kibana site as specified in the waf_elk README.md site.
- Afterwards you'll import the specific settings as by the instrucitons on the README.md file.

That will complete waf_elk.  Next time you open your Virtula Machine. You will need to run start_docker.sh in order to ge the site up and running again. It should look like a variation of this: 

![image](https://github.com/rainyjluke/HoneyHomeLab/assets/119358099/f4dbb793-3c43-44fa-95bb-b79933ca6cfd)
