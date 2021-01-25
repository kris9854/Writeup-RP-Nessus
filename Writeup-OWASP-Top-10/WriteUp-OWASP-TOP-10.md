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


## Task 10: [Severity 3] Sensitive Data Exposure (Supporting Material 2)


## Task 11: [Severity 3] Sensitive Data Exposure (Challenge)


## Task 12: [Severity 4] XML External Entity

## Task 13: [Severity 4 XML External Entity - eXtensible Markup Language


## Task 14: [Severity 4] XML External Entity - DTD


## Task 15: [Severity 4] XML External Entity - XXE Payload

## Task 16: [Severity 4] XML External Entity - Exploiting

## Task 17: [Severity 5] Broken Access Control

## Task 18: [Severity 5] Broken Access Control (IDOR Challenge)
## Task 19: [Severity 6] Security Misconfiguration
## Task 20: [Severity 7] Cross-site Scripting

## Task 21: [Severity 8] Insecure Deserialization
## Task 22: [Severity 8] Insecure Deserialization - Objects

## Task 23: [Severity 8] Insecure Deserialization - Deserialization


## Task 24: [Severity 8] Insecure Deserialization - Cookies

## Task 25: [Severity 8] Insecure Deserialization - Cookies Practical

## Task 26: [Severity 8] Insecure Deserialization - Code Execution

## Task 27:  [Severity 9] Components With Known Vulnerabilities - Intro

## Task 28: [Severity 9] Components With Known Vulnerabilities - Exploit


## Task 29: [Severity 9] Components With Known Vulnerabilities - Lab
## Task 30: [Severity 10] Insufficient Logging and Monitoring
## Task 31: What Next? 
Just Reading


