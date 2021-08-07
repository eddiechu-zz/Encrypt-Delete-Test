# Ransomware kill chain

Recon -> Weaponization -> Delivery -> Exploitation -> Installation -> Command & Control -> Exfiltration

We see many anti-virus / next generation endpoints claim ransomware protection, just can detect and stop invasion, but DO NOT AWARE the encryption process.

Even the vendor sell high ranking, expensive, feature rich, detail EDR and granular control

![alt text](https://i1.wp.com/sandiegofreepress.org/wp-content/uploads/2015/12/gold-toilet-paper.jpg?fit=240%2C210&ssl=1)

Customer still got Ransomeware, most of PC and servers were locked.

They explain you should turn on all block mode, make sure all computer have the endpoint software, keep computer patch up to date, review log regulaerly, follow up abnormal event, then MOST of invasion can be stopped.

How many company in the world can make sure this?  Why it cannot stop encryption after failure invasion detection?


# Which brand can detect encryption process?

That's why I develop this tool.  It is not to replicate found malware, has no footprint in signature, no bias, just do encrypt and delete, simulate the core operation of ransomware.

It is safe enough to run it on your working PC and server, let you see the fact in your environment.

I have helped people to test for several years, luckly, found few brands can detect it, and one of them can stop ransomware encryption initiated from remote PC via file share and RDP as well.  Amazing!


# This tool

This tool encrypts the files under running folder and subfolder, you may create a temperate folder like C:\Encrypt-Delete-Test\, save this tool to there, then run it.  Be safe.

EncryptDelTestv3.jar
- runs on Windows and Mac OS
- requires at least Java 7, http://www.java.com

EncryptDelTestv3.exe
- requires at least .NET Framework 4.0
- runs on Windows


#

Windows screen


![alt text](https://raw.githubusercontent.com/eddiechu/Encrypt-Delete-Test/main/Image/screen01.png)

![alt text](https://raw.githubusercontent.com/eddiechu/Encrypt-Delete-Test/main/Image/screen03.png)


Java screen

![alt text](https://raw.githubusercontent.com/eddiechu/Encrypt-Delete-Test/main/Image/screen04.png)
