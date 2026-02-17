

                                                       Day 1 - Linux Server Setup


- After installing VirtualBox and downloading Ubuntu Server 24.04.4
- Created a VM on which the Ubuntu Server runs
- Created noramal user 'blcstar'
- Updated the system using 'sudo apt update && sudo apt upgrade -y'
- Proceeded by installing the Nginx server and verified that all services were running using 'systemctl status nginx'
- When over to my host machine browser and typed 'http:// localhost' but couldn't see the Nginx welome page, had to do some troubleshooting:
- Under Network, i had to exxposed the VM to the host using NAT port forwarding (Port 8080) alongside the address of the VM
- After all this, i could access the nginx welcome page by typing 'http:// localhost:8080' on the host browser.

