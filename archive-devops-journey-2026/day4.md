

                                           DAY 4 - LINUX NETWORKING & SERVICES 

- systemd is used in Linux to manage services
- the command systemctl list-units --type=service lists all running services on the system
- ss -tulnp command to check for ports and their listening states (t-tcp, u-udp, l-listening, n-numeric, p-process)
- sudo /bin/bash -p permit to access the bash shell as a superuser(root), which is very risky and can be used by those in the sudo group  
- installed and openssh server
- Enabled firewall and allow the ssh services
- disabled password brute force in the sshd_config file using (PasswordRootLogin no), PasswordAuthentication no
- when given a new server, the following must be done:
      - Update the system 
      - Enable firewall and allow only port 22
      - scan for running services and ports
      - install and enable openssh server
      - Disable root password login in the sshd_config file 

