# Really can protect from ransomware encryption?

###### Ransomware attack flow

[Campaign] -> [Infection] -> [Staging] -> [Scan] -> [Encrypt] -> [Payday]

We see many anti-virus / next generation endpoints claim ransomware protection, which can just detect and stop invasion, but CANNOT AWARE the encryption process.

Even those vendors sell high ranking, expensive, feature rich, detail EDR, heuristic detection, AI, ML and granular control, customers still got Ransomware, most of PC and servers were locked.

![alt text](https://raw.githubusercontent.com/eddiechu/Encrypt-Delete-Test/main/Image/screen10.gif)

Vendors usually advise you to turn on all block mode, make sure all computer have the endpoint software installed, keep computer patch up to date, review log regulaerly, follow up abnormal event, then MOST of invasion can be stopped.

How many companies in the world can make sure this?  Why can't it stop encryption after bypass invasion detection?

**Stop encryption is the last defense, which cannot be neglected.**

**Again, top encryption is the last defense, which cannot be neglected.**


# Which brand can detect encryption operation?

That's why I developed this tool.  It is not to replicate found malware, not vendor test tool, no bias, no need to install, just do encrypt and delete, simulate the core operation of ransomware.

It is safe enough to run it on your working PC and server, let you see the fact in your environment.

I have helped people to test this for several years.  Luckly, I found few brands can detect it, and one of them can stop ransomware encryption initiated from remote PC via file share and RDP as well.  I did see a real Ransomware incident, that endpoint really could stop encryption, no loss.

You can refer to the source code if you know programming or you can download the complied files, password zipped or ISO version.

Hope there is no more ransomware incident!  Please share this blog with friends if you found it is useful.


# This tool

This tool encrypts and deletes the files under running folder and subfolder, you may create a temporary folder like C:\Encrypt-Delete-Test\, save this tool to there, then run it.  Be safe.

It is not to test if your endpoint can stop it to open, but to test if your endpoint can detect the encryption is processing.

EncryptDelTestv3.jar
- runs on Windows and Mac OS
- requires at least Java 7, http://www.java.com
(usually java.exe or javaw.exe is a trusted software, it is more difficult for endpoint to detect)


EncryptDelTestv3.exe
- requires at least .NET Framework 4.0
- runs on Windows

| EncryptDelTestv3.jar | EncryptDelTestv3.exe |
|---------------|---------------|
|![alt text](https://raw.githubusercontent.com/eddiechu/Encrypt-Delete-Test/main/Image/screen15.png)|![alt text](https://raw.githubusercontent.com/eddiechu/Encrypt-Delete-Test/main/Image/screen13.png)|


# How it works

###### EncryptDelTestv3.exe (local drive)

| CANNOT detect | CAN detect |
|---------------|---------------|
|![alt text](https://raw.githubusercontent.com/eddiechu/Encrypt-Delete-Test/main/Image/screen10.gif)|![alt text](https://raw.githubusercontent.com/eddiechu/Encrypt-Delete-Test/main/Image/screen13.gif)|
| The tool encrypts all files, a red page is shown and all files are encrypted | The tool is terminated, no red page is shown, few files are encrypted, part of them are being restored |


#

###### EncryptDelTestv3.exe (remote attack)

| CAN detect |
|---------------|
|![alt text](https://raw.githubusercontent.com/eddiechu/Encrypt-Delete-Test/main/Image/screen15.gif)|
|The tool tried to encrypt network drive, server terminated the encryption from remote, few files were encrypted, part of them were being restored|


#

###### EncryptDelTestv3.jar (local drive)

| CANNOT detect | CAN detect |
|---------------|---------------|
|![alt text](https://raw.githubusercontent.com/eddiechu/Encrypt-Delete-Test/main/Image/screen12.gif)|![alt text](https://raw.githubusercontent.com/eddiechu/Encrypt-Delete-Test/main/Image/screen14.gif)|
| The tool encrypted all file, red page shown up and all files were encrypted | The tool was being terminated, no red page shown up, few files were encrypted, part of them were being restored |









#

ransomware test tool
ransomware simulation
ransomware simulator
ransomware assessment
eddie chu
eddiechu.android@gmail.com
anti-ransomware
antivirus test
anti-virus test
endpoint test
infosec
security
cyber security
cybersecurity
incident response
hacker
antimalware
anti-malware
