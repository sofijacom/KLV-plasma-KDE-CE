KLV-Airedale

It seems to work, I need to have someone who knows test it, I don't remember how it works on Airedale :geek:

the configuration file has been slightly modified

in /etc/samba/smb.conf

Код:

#this is a very simple smb.conf to get you started
#coutesy rcrsn51 and gcmartin
[global]
	workgroup = Workgroup
	netbios name = void-live
	server string = KLV-Airedale Server
	security = user
	map to guest = Bad Password
	printing = cups
	printcap name = cups
	load printers = yes
	client min protocol = NT1
        server min protocol = LANMAN1

[klv]
	path = /root/smbvoid
	comment = Shared files
	writable = yes


[printers]
	comment = All Printers
	path = /var/spool/samba
	browseable = no
	guest ok = yes
	writable = no
	printable = yes

--------------------------------------------------------------------------------------

Create a user group:

sudo groupadd -r sambauser
Код: Выделить всё

Add the user1 to the sambauser group:

sudo gpasswd sambauser -a spot
Код: Выделить всё

vNow create samba share user:

sudo smbpasswd -a spot

New SMB password: <input password >
Retype new SMB password: <repeat password>

