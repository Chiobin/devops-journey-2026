

                                  DAY 3 - ADVANCED LINUS PERMISSION(SETUID, SETGID AND STICKY BITS)

-  setuid enables the current user(ruid) to use the previlages of another user attributed to the file (euid) which is usually the root.
-  which use this when there's a need to attribute rights of the owner of a file to other users that might use the same file and permit 
 them to modify it.
-  the numerical value of setuid is 4, which is been placed before the other numerical rights like 4755, chmod u+s.
-  admin need to be very careful while using setuid cos it might lead to previledge escalation through path exploitation, code injection
 or even buffer overflow which can be used by an attacker to get hold of the system
-  setguid permits daughter directories sub directories to carry the previledges of the parent folder, this is mostly used with shared folders
-  setguid also let the daughter directories carry the same group as that of parent just as it was configured
-  the numerical value for setguid is 2, placed before the other rights like 2770 or chmod g+s.
-  sticky bits prevents other user from deleting a file. Only the owner is allowed to do that
-  this is very useful in public folder where veryone has full access over the folder.
-  sticky bits numerical value is 1 and comes before the other rights like, 1777 or 1755.
-  mini lab experiment was carried out in order to test these permissions which worked out just fine.
