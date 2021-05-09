Basic Pentesting

Tyler Imanian
----
ip:10.10.77.23
----
ports:
 22/tcp   open  ssh         OpenSSH 7.2p2 Ubuntu 4ubuntu2.4 (Ubuntu Linux; protocol 2.0)
 | ssh-hostkey: 
 |   2048 db:45:cb:be:4a:8b:71:f8:e9:31:42:ae:ff:f8:45:e4 (RSA)
 |   256 09:b9:b9:1c:e0:bf:0e:1c:6f:7f:fe:8e:5f:20:1b:ce (ECDSA)
 |_  256 a5:68:2b:22:5f:98:4a:62:21:3d:a2:e2:c5:a9:f7:c2 (ED25519)
 80/tcp   open  http        Apache httpd 2.4.18 ((Ubuntu))
 |_http-server-header: Apache/2.4.18 (Ubuntu)
 |_http-title: Site doesn't have a title (text/html).
 139/tcp  open  netbios-ssn Samba smbd 3.X - 4.X (workgroup: WORKGROUP)
 445/tcp  open  netbios-ssn Samba smbd 4.3.11-Ubuntu (workgroup: WORKGROUP)
 8009/tcp open  ajp13?
 |_ajp-methods: Failed to get a valid response for the OPTION request
 8080/tcp open  http-proxy
----
notes:
	look at smb to find  username, enum4linux command 
		users found jan, kay
	looking through jan files you can go to home and see /kay and in /kay you find a pass.bak which has her password
	no need to use the exploit I found.
----
What is the name of the hidden directory on the web server(enter name without /)?
	development
----
What is the username? 
	jan 
----
What is the password? 
	armando
----
What service do you use to access the server(answer in abbreviation in all caps)? 
 	SSH
----
What is the name of the other user you found(all lower case)? 
	kay
----
What is the final password you obtain? 
	heresareallystrongpasswordthatfollowsthepasswordpolicy$$
----

