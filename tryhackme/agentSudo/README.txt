Agent Sudo

Tyler Imanian
----
ip:10.10.57.140
----
ports:
21/tcp open  ftp     vsftpd 3.0.3
22/tcp open  ssh     OpenSSH 7.6p1 Ubuntu 4ubuntu0.3 (Ubuntu Linux; protocol 2.0)
80/tcp open  http    Apache httpd 2.4.29 ((Ubuntu))
----
notes:
	some hard hints to use user agent stuff (had to look up how to use it but its easy to use)

	use steghide and binwalk to look at .jpeg/.png

	found a zip pass in the png: alien
	base 64 pass: QXJlYTUx = Area51
	.jpeg hide the name james and the pass hackerrules!
----
How many open ports?
	3
----
How you redirect yourself to a secret page?
	user-agent
----
What is the agent name?
	chris
----
FTP password
	crystal
----
Zip file password
	alien
----
steg password
	Area51
----
Who is the other agent (in full name)?
	james
----
What is the user flag?
b03d975e8c92a7c04146cfa7a5a313c7
----
what is the incident of the photo called?
	Roswell alien autopsy
----
CVE number for the escalation 
	CVE-2019-14287
----
What is the root flag?
	b53a02f55b57d4439e3341834d70c062
----
(Bonus) Who is Agent R?
	DesKel
----
