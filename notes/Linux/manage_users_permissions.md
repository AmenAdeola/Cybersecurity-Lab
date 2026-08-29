# Manage Users and their Permissions

Command | Purpose | Example
--------|---------|--------
chmod | Changes/modify permissions on files and directories | chmod u+rwx,g+rwx,o+rwx login_sessions.txt: Changes user (u), group (g), and other (o) permissions to add (+) read (r), write (w), and execute (x) permissions for the login_sessions.txt file; chmod g-rw bonuses.txt: Changes the group (g) permissions to remove (-) read (r) and write (w) permissions for the bonuses.txt file; chmod u=r,g=r,o=r login_sessions.txt: Changes user (u), group (g), and other (o) permissions to assign (=) read (r) permissions for the login_sessions.txt file
chown | Changes ownership of a file or directory; used with sudo | sudo chown fgarcia access.txt: Changes the user owner of the access.txt file to fgarcia; sudo chown :security access.txt: Changes the group owner of access.txt to security; a colon (:) must be entered before the group name
chown user:group | change owner and group| sudo chown researcher9:research_team project_r.txt
chgrp | Change group ownership | sudo chgrp research_team project_r.txt
groupdel | Deletes a group from the system; used with sudo | sudo groupdel accounting: Deletes accounting as a group
sudo | Temporarily grants elevated permissions to specific users; users must be in a sudoers file to use have access to sudo| sudo useradd fgarcia: Grants elevated permissions to the user running this command and so that this user can use the useradd command to add fgarcia as a new user to the system
useradd | Adds/creates user to the system; used with sudo | sudo useradd fgarcia: Adds fgarcia as a new user to the system; sudo useradd -g security fgarcia: Adds fgarcia as a new user and uses the -g option to set their primary group as security; sudo useradd -G finance,admin fgarcia: Adds fgarcia as a new user and uses the -G option to add them to the supplemental groups of finance and admin
userdel | Deletes a user from the system; used with sudo | sudo userdel fgarcia: Deletes fgarcia as a user; sudo userdel -r fgarcia: Deletes fgarcia as a user and deletes all files in their home directory
usermod | Modifies existing user accounts; used with sudo| sudo usermod -g executive fgarcia:Uses the -g option to set primary group or change the existing fgarcia user's primary group to the executive group; sudo usermod -G accounting fgarcia:Uses the -G option to replace any supplemental groups the the existing fgarcia user is in with the supplemental accounting group; removes all other supplemental groups fgarcia is in;  sudo usermod -a -G marketing fgarcia:Uses the -a -G options to add the existing fgarcia user to the supplemental marketing group; does not remove fgarcia from other supplemental groups;  sudo usermod -d /home/garcia_f fgarcia:Uses the -d option to change theexisting fgarcia user's home directory to /home/garcia_f
stat | Display file metadata and permissions | stat report.txt






