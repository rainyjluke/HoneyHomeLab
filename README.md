# HoneyHomeLab
A Kali Linux customized WAF using template from ModSecurity, with modifications for own specific needs. Purpose of this homelab is to create a offensive penetration testing lab
that has some defensive capabilities that can be modified for your own person needs. For the version listed below, I will be using Oracle VirtualBox with a KaliLinux OS.

# Homelab Specifications:
Use the latest Kali Linux installer for your VirtualBox or Virtual Machine:
  - Base Memory 4080 MB
  - Processor: 5 CPU (you'll need that extra power for the Honeypot that will be installed later)
  - Disk Size: 50 MB (I have done this with the defualt 25MB, but the specific honeypot will use too much disk space. Doubling is more than enough for when in use.)
Follow the prompts that it will ask you: country, lanugage, GUI interface, timezone all that good stuff. After answering the preliminary questions, it will start to install and set up. The installation will take some time, so keep your computer on as the VirtualBox installs.

# Honeypot Installation:
For this honeypot we will be using the OWASP Honeypot found at https://github.com/OWASP/Honeypot-Project
  - Start by opening a terminal and using the following command:

    sudo git clone --recurse-submodules https://github.com/OWASP/Honeypot-Project.git
  
  - Once that is done in the directory of your choosing go to honeytraps directory:
    
    cd Honeypot-Projects/honeytrap
  
  - From there you will go ahead and read the README.md of each directory. They will have more information and specifications on how to set each directory up.
  - I started with misp, then waf_elk, and then waf_modsec. It is the most straightforward sequence that will acheive the desired results.
