## Shell Permissions Project

**Task 0:** su betty **:** changes your user ID to betty.

**Task 1:** id -un **:** Print the user ID of current user. alternative is whoami

**Task 2:** id -Gn **:** Prints all the groups the current user is part of.

**Task 3:** chown betty hello **:** Changes the owner of the file hello to the user betty

**Task 4:** touch hello **:** Create an empty file called hello

**Task 5:** chmod u+x hello **:** Add execute permission to the owner of the file hello

**Task 6:** chmod ug+x,o+r **:** hello Add execute permission to user and group owner, and read permission to others for file hello

**Task 7:** chmod ugo+x **:** hello Add execution permission to all for file hello.

**Task 8:** chmod 007 hello **:** Set permissions for file hello so owner and group don't have any permissions and other users have all permissions.

**Task 9:** chmod 753 hello **:** Set permissions so owner has all permissions, group has read and execute permissions and others have write and execute permissions.

**Task 10:** chmod --reference=olleh hello **:** Copies the mode of file olleh to file hello.

**Task 11:** chmod -R +X . **:** Add execute permission to all subdirectories of the current directory for the everyone. Regular files should not be changed.

**Task 12:** mkdir -m 751 my_dir **:** Create a directory called my_dir with permissions 751. User has all read, write, and execute permissions. Group has read and execute permissions. Others have just execute permission.

**Task 13:** chgrp school hello **:** Change group owner to school for the file hello

**Task 14:** chown vincent**:**staff * **:** Change owner to vincent and the group owner to staff for all files and directories in current directory.

**Task 15:** chown -h vincent**:**staff _hello **:** Changes the owner and group owner of file _hello to vincent and staff respectively.

**Task 16:** chown --from=guillaume betty hello **:** Change owner of the file hello to betty only if it is currently owned by guillaume

**Task 17:** telnet towel.blinkenlights.nl Play **:** the Star Wars IV episode in the terminal. This is a premade script provided online.

