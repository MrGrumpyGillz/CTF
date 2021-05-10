Simple CTF

Tyler Imanian
----
ip:10.10.177.42
----
ports:
21/tcp   open  ftp     vsftpd 3.0.3
80/tcp   open  http    Apache httpd 2.4.18 ((Ubuntu))
2222/tcp open  ssh     OpenSSH 7.2p2 Ubuntu ubuntu2.8 (Ubuntu Linux; protocol 2.0)
----
notes:
	updated the exploit to work with python3 syntax

----
How many services are running under port 1000?
	2
----
What is running on the higher port?
	ssh
----
What's the CVE you're using against the application? 
	cve-2019-9053 (CVE:2019-9053 format did not work and gave me some trouble, was actually last thing I answered)
----
To what kind of vulnerability is the application vulnerable?
	sql injection (sqli)
----
What's the password?
	secret
----
Where can you login with the details obtained?
	ssh
----
What's the user flag?
	G00d j0b, keep up!
----
Is there any other user in the home directory? What's its name?
	sunbath
----
What can you leverage to spawn a privileged shell?
	vim (has use of vim -c ':!/bin/sh')
----
What's the root flag?
	W3ll d0n3. You made it!
----
