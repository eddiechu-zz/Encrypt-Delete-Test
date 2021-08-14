# Really can protect from ransomware encryption?

###### Ransomware attack flow

[Campaign] -> [Infection] -> [Staging] -> [Scan] -> [Encrypt] -> [Payday]

We see many anti-virus / next generation endpoints claim ransomware protection, which can just detect and stop invasion, but CANNOT AWARE the encryption process.

Even those vendors sell high ranking, expensive, feature rich, detail EDR, heuristic detection, AI, ML and granular control, customers still got Ransomware, most of PC and servers were locked.

![alt text](https://raw.githubusercontent.com/eddiechu/Encrypt-Delete-Test/main/Image/screen10.gif)

Vendors usually advise you to turn on all block mode, make sure all computer have the endpoint software installed, keep computer patch up to date, review log regulaerly, follow up abnormal event, then MOST of invasion can be stopped.

How many companies in the world can make sure this?  Why can't it stop encryption after bypass invasion detection?

##Stop encryption is the last defense, cannot be neglected.


# Which brand can detect encryption operation?

That's why I developed this tool.  It is not to replicate found malware, not vendor test tool, no bias, just do encrypt and delete, simulate the core operation of ransomware.

It is safe enough to run it on your working PC and server, let you see the fact in your environment.

I have helped people to test this for several years.  Luckly, I found few brands can detect it, and one of them can stop ransomware encryption initiated from remote PC via file share and RDP as well.  I did see a real Ransomware incident, that endpoint really could stop encryption, no loss.


# This tool

This tool encrypts the files under running folder and subfolder, you may create a temporary folder like C:\Encrypt-Delete-Test\, save this tool to there, then run it.  Be safe.

The principle is not to test if your endpoint can stop the tool to start, but to test if the endpoint can detect and stop the tool when the encryption is processing.

EncryptDelTestv3.jar
- runs on Windows and Mac OS
- requires at least Java 7, http://www.java.com
(usually java.exe is a trusted software, it is more difficult for endpoint to safegard)


EncryptDelTestv3.exe
- requires at least .NET Framework 4.0
- runs on Windows

| EncryptDelTestv3.jar | EncryptDelTestv3.exe |
|---------------|---------------|
|![alt text](https://raw.githubusercontent.com/eddiechu/Encrypt-Delete-Test/main/Image/screen15.png)|![alt text](https://raw.githubusercontent.com/eddiechu/Encrypt-Delete-Test/main/Image/screen13.png)|


# Test cases

###### Windows (local drive)

| CANNOT detect | CAN detect |
|---------------|---------------|
|![alt text](https://raw.githubusercontent.com/eddiechu/Encrypt-Delete-Test/main/Image/screen10.gif)|![alt text](https://raw.githubusercontent.com/eddiechu/Encrypt-Delete-Test/main/Image/screen13.gif)|
| The tool encrypts all file, red page show up and all files are encrypted | The tool being terminated, no red page show up, few files are encrypted, part of them are being restored |


#

###### Windows (remote attack)

| CAN detect |
|---------------|
|![alt text](https://raw.githubusercontent.com/eddiechu/Encrypt-Delete-Test/main/Image/screen15.gif)|
|The tool encrypt network drive, server terminated the remote operation, few files are encrypted, part of them are being restored|


#

###### Java (local drive)

| CANNOT detect | CAN detect |
|---------------|---------------|
|![alt text](https://raw.githubusercontent.com/eddiechu/Encrypt-Delete-Test/main/Image/screen12.gif)|![alt text](https://raw.githubusercontent.com/eddiechu/Encrypt-Delete-Test/main/Image/screen14.gif)|
| The tool encrypts all file, red page show up and all files are encrypted | The tool being terminated, no red page show up, few files are encrypted, part of them are being restored |






#ransomware
#test
#tool
