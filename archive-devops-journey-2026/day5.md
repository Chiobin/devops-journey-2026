

                                               DAY 5 - NGINX WEB SEERVER CONFIGURATION AND SITE HOSTING 

- Recall on the first, i installed and deployed the nginx server, it was time to secure and learn how to host multiple websites on the server
- started by creating a folder in myapp in /var/www/, then proceeded by changing the rights using sudo chown -R root:root /var/www/myapp
- sudo chmod -R 755 /var/www/myapp. myapp contained a single html file.
- managed /etc/nginx/sites-available and sites-enabled.
- sudo nano /etc/nginx/sites-available/myapp, where i conigured my server_name, port to listen, file to load and location.
- sudo ln -s /etc/nginx/sites-enabled/.
- ran sudo nginx -t to make sure everything is working properly which returned ok
- allowed port 80 on the firewall
- Given that the server ia running on a VM and uses NAT, i had to forward the port so that the file can be accessed by my host machine
- curl localhost:80 on the server to make sure the index file hass a return
- the ran the http://localhost:80 which worked successfully
- did same for the other static html sites; myapp2 and myapp3 with their respective ports 8080 and 8081.
- troubleshoot git connection severed; installed keychain and configured so as not to be asked for authentication each time i need to do a push.
