# Really protect from ransomware encryption?
We see many anti-virus / next generation endpoints claim ransomware protection, they are high ranking, expensive, feature rich, detail EDR and granular control

![alt text](https://i1.wp.com/sandiegofreepress.org/wp-content/uploads/2015/12/gold-toilet-paper.jpg?fit=240%2C210&ssl=1)

 BUT CANNOT detect ransomware encryption operation, whole office computers and servers being locked.

Those vendors explain you should turn on all block mode, make sure all computer have the endpoint software, keep computer patch up to date, review log regulaerly, follow up abnormal event, then most of invasion can be stopped.

How many company in the world can make sure this.

# Which brand can really protect?

That's why I develop this tool.  It is not to replicate found malware, has no footprint in signature, just do encrypt and delete, simulate the core operation of ransomware.

It is safe enough to run it on your working PC and server, let you see the fact in your environment.

Luckly, I found few brands can do, and one of them can stop ransomware encryption initiated from remote PC via file share and RDP as well.  Amazing!

# Caution

This tool encrypts the files under running folder and subfolder, you may create a temperate folder like C:\Encrypt-Delete-Test\, save this tool to there, then run it.  Be safe.

# This tool

EncryptDelTestv3.jar
- runs on Windows and Mac OS
- requires at least Java 7, http://www.java.com

EncryptDelTestv3.exe
- requires at least .NET Framework 4.0
- runs on Windows

Windows screen


![alt text](https://raw.githubusercontent.com/eddiechu/Encrypt-Delete-Test/main/Image/screen01.png)

![alt text](https://raw.githubusercontent.com/eddiechu/Encrypt-Delete-Test/main/Image/screen03.png)


Java screen

![alt text](https://raw.githubusercontent.com/eddiechu/Encrypt-Delete-Test/main/Image/screen04.png)
