# 7330: Computer and Network Security Homework 5
## Matthew Reheuser 
#### 2023.10.29 <p>&nbsp;</p>


1. Redhat Academy work [4 points]   
• Take a screenshot of step #6 in Section 10.2 Guided exercise.  
This screenshot is showing the current computers and users that are connected using ssh.  
![10.2#6](./pictures/10.2-Q6.png)  
• Take a screenshot of step #12 in Section 10.2 Guided exercise.  
This is a means of connecting to serverb without having to enter the shell. This is demonstrating that I have access to serverb without having to input a password. The host key of serverb in the known_hosts folder.   
![10.2#12](./pictures/10.2-Q12.png)  
• Take a screenshot of step #4 in Section 10.4 Guided exercise.  
This is sending the ssh key to the user operator1 on the servera. Giving me access to servera as operator1 without having to enter a password.
![10.4#4](./pictures/10.4-Q4.png)  
• Take a screenshot of step #9 in Section 10.4 Guided exercise.  
When creating an ssh key pair they can be password protected as shown below. That password is different than the password of the operator1 on servera, therefore you would need two distinct passwords to get in. 
![10.4#9](./pictures/10.4-Q9.png)  



2. NUC ssh key work [3.5 points]  
• Generate your own SSH keys  
Used ssh-keygen to create a ssh key pair.
![Generate SSH](./pictures/3GenerateSSH.png)  
• Share your public key to the Cybernet jump box from lab 6  
Windows does not have as simple as a solution for sharing ssh keys so I used scp to copy the id_rsa.pub file into the .ssh/authorized_keys folder on the jump box. First I needed to generate a key on the jump box to create the folder structure for an authorized key which I then deleted before transfering over the key.
![ssh share key](./pictures/3ShareKey.png)  
• Login as your user using key based authentication  
I was able to login without the need for a password, meaning the ssh keys worked.
![ssh login](./pictures/3Login.png)  


3. Brute force work [1.5 points]
    1. Login to the jumpbox using your user name from Lab 6. Change the password using the passwd command to a password that exists in the password list.  
    Changed the password to matthew, as it was a part of the top 100 passwords list.
    ![change password](./pictures/password.png)  
    2. Use your existing user name as the user to brute for passwords. Depending on the tool, this may mean creating a “list” file of one user or providing the user name on the command line.  
    Created the username "list" being just my single username.  
    ![usernames](./pictures/Usernames.png)  
    3. Run your tool of choice (see notes) against the jumpbox to “discover” the password.  
    This started at the top of the password list and attempted different password combitations until one succeded. Then telling the user the matching password ans username. 
    ![brute force](./pictures/Bruteforce.png)  



