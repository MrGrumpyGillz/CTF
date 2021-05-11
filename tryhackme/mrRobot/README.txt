Mr. Robot CTF

Tyler Imanian
----
ip:10.10.234.95
----
ports:
22/tcp  closed ssh
80/tcp  open   http     Apache httpd
443/tcp open   ssl/http Apache httpd
----
notes:
	has an ssl cert: commonName=www.example.com , might be self signed and can be abused
	found that this runs on a wordpress site
	found that robot.txt give you the first key (used nikto and found vuln in file system), also found a .dic file
	brute forcing the wp website using wpscan: Using some meta knowlege I assume the user is elliot from the show. and you find the password for him: user: elliot pass: ER28-0652
	make a webpage that give you a root shell is probably the best thing to do now.
	found a user flag as the 2nd key

	could never find a way to get last flag:
	In the write up they found a vuln in nmap where you can run a shell from --interactive 
----
key 1:
	073403c8a58a1f80d943455fb30724b9
----
key 2:
	822c73956184f694993bede3eb39f959
----
key 3:
	04787ddef27c3dee1ee161b21670b4e4 
----