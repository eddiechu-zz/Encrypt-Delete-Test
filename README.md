# Ransomware kill chain

Recon -> Weaponization -> Delivery -> Exploitation -> Installation -> Command & Control -> Exfiltration

We see many anti-virus / next generation endpoints claim ransomware protection, which can just detect and stop invasion, but CANNOT AWARE the encryption process.

Even those vendors sell high ranking, expensive, feature rich, detail EDR and granular control,

[![Most Expensive Useless Things](https://i.ytimg.com/vi/6Q5nrnyWqyM/maxresdefault.jpg)](https://www.youtube.com/watch?v=6Q5nrnyWqyM)

customers still got Ransomware, most of PC and servers were locked.

Vendors usually advise you to turn on all block mode, make sure all computer have the endpoint software installed, keep computer patch up to date, review log regulaerly, follow up abnormal event, then MOST of invasion can be stopped.

How many companies in the world can make sure this?  Why can't it stop encryption after bypass invasion detection?


# Which brand can detect encryption operation?

That's why I developed this tool.  It is not to replicate found malware, not vendor test tool, no bias, just do encrypt and delete, simulate the core operation of ransomware.

It is safe enough to run it on your working PC and server, let you see the fact in your environment.

I have helped people to test this for several years.  Luckly, I found few brands can detect it, and one of them can stop ransomware encryption initiated from remote PC via file share and RDP as well.  I did see a real Ransomware incident, that endpoint really could stop encryption, no loss.


# This tool

This tool encrypts the files under running folder and subfolder, you may create a temporary folder like C:\Encrypt-Delete-Test\, save this tool to there, then run it.  Be safe.

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


#

Java screen

![alt text](https://raw.githubusercontent.com/eddiechu/Encrypt-Delete-Test/main/Image/screen04.png)
