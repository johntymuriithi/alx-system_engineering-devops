su changes user to the specified one
whoami command prints out the name of the current user
group = command prints out the groups that the cureent user is part of
sudo chown command changes the ownership of a file
touch command creats an empty file
chmod 700 file_name command gives permmisions of execution to the owner of a certain file
chmod u+x,g+x,o+r hello gives persion to user groupp and owner to execute file
chmod 751 hello command permits execution of hello file to user owner and the group
chmod 007 hello command permits all permissions to the users
chmod 751 added
chmod 751 cretes create directory with 751 permissions
chmod --reference=olleh hello sets permisions of ollen as hello
find . -type d -exec chmod +x {} + command adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users.
chown :school hello command that changes the group owner to school for the file hello
sudo chown -R vincent:staff . commands changes the owner to vincent and the group owner to staff for all the files and directories in the working directory.
sudo chown -h vincent:staff _hello command changes the owner and the group owner of _hello to vincent and staff respectively.
if [ "$(stat -c '%U' hello)" = "guillaume" ]; then sudo chown betty hello; fi command changes the owner of the file hello to betty only if it is owned by the user guillaume
