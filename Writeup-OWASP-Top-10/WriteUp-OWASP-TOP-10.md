# TryhackMe: OWASP Top 10

Part of tryhackme's "Complete Beginner" path

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
Command: 
<br/>
Answer:
### 7.2
Now try to do the same trick and see if you can login as arthur.
<br/>
Answer: NULL

### 7.3
What is the flag that you found in arthur's account?
<br/>
Answer: 

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
Command:
<br/>
Answer:

### 11.2
Navigate to the directory you found in question one. What file stands out as being likely to contain sensitive data?
<br/>
Command:
<br/>
Answer:

### 11.3
Use the supporting material to access the sensitive data. What is the password hash of the admin user?
<br/>
Command:
<br/>
Answer:

### 11.4
What is the admin's plaintext password?
<br/>
Command:
<br/>
Answer:

### 11.5
Login as the admin. What is the flag?
<br/>
Command:
<br/>
Answer:

## Task 12: [Severity 4] XML External Entity
Just Reading and deploying machine
## Task 13: [Severity 4 XML External Entity - eXtensible Markup Language
### 13.1
Full form of XML
<br/>
Answer:

### 13.2
Is it compulsory to have XML prolog in XML documents?
<br/>
Answer: no

### 13.3
Can we validate XML documents against a schema?
<br/>
Answer:

### 13.4
How can we specify XML version and encoding in XML document?
<br/>
Answer:

## Task 14: [Severity 4] XML External Entity - DTD
### 14.1
How do you define a new ELEMENT?
<br/>
Answer:

### 14.2
How do you define a ROOT element?
<br/>
Answer:

### 14.3
How do you define a new ENTITY?
<br/>
Answer:

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
Answer:

### 16.4
Where is falcon's SSH key located?
<br/>
Answer:

### 16.5
What are the first 18 characters for falcon's private key
<br/>
Answer:


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
Answer:

## Task 19: [Severity 6] Security Misconfiguration
### 19.1
Deploy the VM
<br/>
Answer: Completed without answer

### 19.2
Hack into the webapp, and find the flag!
<br/>
Answer: 

## Task 20: [Severity 7] Cross-site Scripting


### 20.1
Deploy the VM
<br/>
Answer: Completed without answer

### 20.2

Navigate to http://MACHINE_IP/ in your browser and click on the "Reflected XSS" tab on the navbar; craft a reflected XSS payload that will cause a popup saying "Hello".
<br/>
Answer: 

### 20.3
On the same reflective page, craft a reflected XSS payload that will cause a popup with your machines IP address.
<br/>
Answer: 

### 20.4
Then add a comment and see if you can insert some of your own HTML.
<br/>
Answer: 

### 20.5
On the same page, create an alert popup box appear on the page with your document cookies.
<br/>
Answer: 

### 20.6
Change "XSS Playground" to "I am a hacker" by adding a comment and using Javascript.
<br/>
Answer: 


## Task 21: [Severity 8] Insecure Deserialization
### 21.1
Who developed the Tomcat application?
<br/>
Answer: 

### 21.2
What type of attack that crashes services can be performed with insecure deserialization?
<br/>
Answer:

## Task 22: [Severity 8] Insecure Deserialization - Objects
## 22.1
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
Answer:

## Task 24: [Severity 8] Insecure Deserialization - Cookies
### 24.1
If a cookie had the path of webapp.com/login , what would the URL that the user has to visit be?
<br/>
Answer:

### 24.2
What is the acronym for the web technology that Secure cookies work over?
<br/>
Answer:
## Task 25: [Severity 8] Insecure Deserialization - Cookies Practical
### 25.1
1st flag (cookie value)
<br/>
Answer:

### 25.2
2nd flag (admin dashboard)
<br/>
Answer:
## Task 26: [Severity 8] Insecure Deserialization - Code Execution
### 26.1
flag.txt
<br/>
Answer:
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

### 30.2
What kind of attack is being carried out?
<br/>
Answer: brute force
## Task 31: What Next? 
Just Reading


