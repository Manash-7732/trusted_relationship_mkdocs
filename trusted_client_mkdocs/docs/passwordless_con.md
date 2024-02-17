# Creating public and private key pair on the server and importing the private key to the client for making password less connection

## To create public key on the server and import private key 

* Login into PuTTY and type the command ssh-keygen -b 1024 -t rsa
* With the help of cd .ssh/ change the directory
* Use ls to list the files created on the server as: authorized_keys id_rsa id_rsa.pub known_hosts
* To save the public key use cat id_rsa.pub and paste it in the authorized_keys file using vi authorized_keys  

## Connect with the private key generated using PuTTYgen 

* In the 'Connection' -> 'SSH' -> 'Auth' category, browse and select the private key file you saved .
* Save these settings if you want to use them again in the future.
* Click 'Open' to establish the SSH connection to the server for keyless authentication.
