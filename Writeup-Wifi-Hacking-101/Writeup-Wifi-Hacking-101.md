# Wifi Hacking 101
Writeup of tryhacksme "wifihacking101" created by NinjaJc01
writen by kris9854

## The basics - An intro to WPA

### What type of attack on the encryption can you perform on WPA(2) personal?
Answer: brute force
### Can this method be used to attack WPA2-EAP handshakes? (Yea/Nay)
Answer: Nay
### What three letter abbreviation is the technical term for the "wifi code/password/passphrase"?
Answer: PSK
### What's the minimum length of a WPA2 Personal password?
Answer: 8

## You're being watched - Capturing packets to attack

### How do you put the interface “wlan0” into monitor mode with Aircrack tools? (Full command)
Answer: airmon-ng wlan0 start
### What is the new interface name likely to be after you enable monitor mode?
Answer: wlan0mon
### What do you do if other processes are currently trying to use that network adapter? 
Answer: airmon-ng check kill
### What tool from the aircrack-ng suite is used to create a capture?
Answer: airodump-ng

### What flag do you use to set the BSSID to monitor?
Answer: --bssid
### And to set the channel?
Answer: --channel
### And how do you tell it to capture packets to a file?
Answer: -w

## Aircrack-ng - Let's Get Cracking
###What flag do we use to specify a BSSID to attack?
Anser: -b
### What flag do we use to specify a wordlist?
Answer: -w
### How do we create a HCCAPX in order to use hashcat to crack the password?
Answer: -j
### Using the rockyou wordlist, crack the password in the attached capture. What's the password?
Answer: greeneggsandham
<br/>
command used - "aircrack-ng -b 02:1A:11:FF:D9:BD -w /usr/share/wordlists/rockyou.txt -l key.txt NinjaJc01-01.cap"
### Where is password cracking likely to be fastest, CPU or GPU?
Answer: GPU