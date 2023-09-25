Create a User:
This was done by using sudo useradd username
![](image_step1.png)

Set an expiry date of 2 weeks for the user:
This was done by using sudo usermod -e YYYY-MM-DD
![](image_step2.png)

Prompt the user to change password on login:
This was done using sudo passwd -e username
![](image_step3.png)

User being asked to change password
![](image_step3.1.png)

Attach the user to a group called altschool:
First, i created altschool group using; 
sudo groupadd gropname.
Then i added the user to the group using;
sudo usermod -aG groupname username
![](image_step4.png)

Allow altschool grop to run only cat command:
This was done by editing the sudoers file.
1: sudo visudo.
2: %groupname All=(All) /bin/cat/etc
![](image_step5.png)

Create another user without home directory:
This was done using sudo useradd -M username
![](image_step6.png)

  