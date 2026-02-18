




                                                          Day 2 - Permissions in Linux


-  Continued from where i ended yesterday, added a new user devopsstudent access index.html in /var/www/html/index.html but couldn't modified
-  That was beacuse the folder html didn't allow for modification rights to others.
-  Inorder to solve the issue, i changed the html folder group from root to www-data
-  Added devopsstudent to www-data using the command "sudo usermod -aG www-data devopsstudent" which permitted him to be added without initializing his groups
-  Then i could modify the index file thanks to the rw attributed to the group
-  Learnt commands with regards to permission and ownership like: 
        - sudo chgrp to change a group ex; www-data /var/www/html
        - sudo chown root:devops
        - chmod 755 (u: rwx g: r-x o: r-x), the user can read, write and modify files, group and others can only read and execute files
        - chmod 750 (u: rwx g: r-x o: none), here others have no rights whereas the user has full rights and the group can only execute and read files
        - chmod 711 (u: rwx g: x o: x)
- Also learnt that if you don't have the r-x rights, can't list files in a folder but can open a file if you know the name cos there's a read permission on that file
- If you add s rights to group, any file created in that folder can be accessible and modified by those in that group: the file is automatically attributed to the group of the folder, this is mostly used in shared folders 
