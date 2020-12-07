# TryhackMe: RP:nessus Writeup

## Task 1:

### Task 1.1:

Deploy the vulnerable machine! This one, well, it has problems.
Deploy the virtual machine!
<br/>
Answer: <span style="text-decoration:underline"> No answer needed </span>

## Task 2:

### Task 2.1:

First, create a basic Ubuntu box (or any other system of your choice). Minimum 4 2GHz cores, 4 GB RAM (8 Recommended) and 30 GB of disk space.
<br/>
Answer: <span style="text-decoration:underline"> No answer needed </span>

### Task 2.2

Next, go ahead and register for a Nessus Home license. This can be used to scan up to 16 IP addresses at a time. Be sure to keep this license information safe, you'll need it for any manual work. Here's the registration link: https://www.tenable.com/products/nessus-home
<br/>
Answer: <span style="text-decoration:underline"> No answer needed </span>

### Task 2.3

Follow the installation instructions on Tenable's website, once Nessus is set up connect the machine that it lives on to the network using your VPN file.
<br/>
Answer: <span style="text-decoration:underline"> No answer needed </span>

## Task 3:

### Task 3.1:

As we log into Nessus, we are greeted with a button to launch a scan, what is the name of this button?
<br/>
Answer: <span style="text-decoration:underline"> New Scan </span>

### Task 3.2:

Nessus allows us to create custom templates that can be used during the scan selection as additional scan types, what is the name of the menu where we can set these?
<br/>
Answer: <span style="text-decoration:underline"> Policies </span>

### Task 3.3:

Nessus also allows us to change plugin properties such as hiding them or changing their severity, what menu allows us to change this?
<br/>
Answer: <span style="text-decoration:underline"> Plugin Rules </span>

### Task 3.4:

Nessus can also be run through multiple 'Scanners' where multiple installations can work together to complete scans or run scans on remote networks, what menu allows us to see all of these installations?
<br/>
Answer: <span style="text-decoration:underline"> Scanners </span>

### Task 3.5:

Let's move onto the scan types, what scan allows us to see simply what hosts are 'alive'?
<br/>
Answer: <span style="text-decoration:underline"> Host Discovery </span>

### Task 3.6:

One of the most useful scan types, which is considered to be 'suitable for any host'?
<br/>
Answer: <span style="text-decoration:underline"> Basic Network Scan </span>

### Task 3.7:

Following a few basic scans, it's often useful to run a scan wherein the scanner can authenticate to systems and evaluate their patching level. What scan allows you to do this?
<br/>
Answer: <span style="text-decoration:underline"> Credentialed Patch Audit </span>

### Task 3.8:

When performing Web App tests it's often useful to run which scan? This can be incredibly useful when also using nitko, zap, and burp to gain a full picture of an application.
<br/>
Answer: <span style="text-decoration:underline"> Web Application Tests </span>

## Task 4:

### Task 4.1:

Deploy the machine and connect to the network
<br/>
Answer: <span style="text-decoration:underline"> No answer needed </span>

### Task 4.2:

Create a new 'Basic Network Scan' targeting the deployed VM. What option can we set under 'BASIC' to set a time for this scan to run? This can be very useful when network congestion is an issue.
<br/>
Answer: <span style="text-decoration:underline"> Schedule </span>

### Task 4.3:

Under discovery set the scan to cover ports 1-65535. What is this type called?
<br/>
Answer: <span style="text-decoration:underline"> Port scan (all ports) </span>

### Task 4.4:

As we are connected to the network via a VPN, it may be to our benefit to 'tone down' the scan a bit. What scan type can we change to under 'ADVANCED' for this lower bandwidth connection?
<br/>
Answer: <span style="text-decoration:underline"> Scan low bandwidth links </span>

### Task 4.5:

With these options set (other than the time to run) save and launch the scan.
<br/>
Answer: <span style="text-decoration:underline"> No answer needed </span>

### Task 4.6:

After the scan completes, which 'Vulnerability' can we view the details of to see the open ports on this host?
<br/>
Answer: <span style="text-decoration:underline"> Nessus SYN scanner </span>

### Task 4.7:

There seems to be a chat server running on this machine, what port is it on?
<br/>
Answer: <span style="text-decoration:underline"> 6667 </span>

### Task 4.8:

Looks like we have a medium level vulnerability relating to SSH, what is this vulnerability named?
<br/>
Answer: <span style="text-decoration:underline"> SSH Weak Algorithms Supported </span>

### Task 4.9:

What web server type and version is reported by Nessus?
<br/>
Answer: <span style="text-decoration:underline"> Apache/2.4.99 </span>

## Task 5:

### Task 5.1

Add SMTP functionality into your Nessus install!
An optional but awesome additional step, link your Nessus box up to an SMTP server via the Settings panel. Google provides this for free if you already have a Gmail account. Adding 2-factor authentication on your account and create an app password, then link Nessus to the Gmail SMTP server via these following settings: https://www.siteground.com/kb/google_free_smtp_server/
<br/>
Answer: <span style="text-decoration:underline"> No answer needed </span>

## Task 6:

### Task 6.1:

Run a web application scan against this new box.
<br/>
Answer: <span style="text-decoration:underline"> No answer needed </span>

### Task 6.2:

What is the plugin id of the plugin that determines the HTTP server type and version?
<br/>
Answer: <span style="text-decoration:underline"> 10107 </span>

### Task 6.3:

What authentication page is discovered by the scanner that transmits credentials in cleartext?
<br/>
Answer: <span style="text-decoration:underline"> /login.php </span>

### Task 6.4:

What is the file extension of the config backup?
<br/>
Answer: <span style="text-decoration:underline"> .bak </span>

### Task 6.5:

Which directory contains example documents? (This will be in a php directory)
<br/>
Answer: <span style="text-decoration:underline"> /external/phpids/0.6/docs/examples/ </span>

### Task 6.6:

What vulnerability is this application susceptible to that is associated with X-Frame-Options?
<br/>
Answer: <span style="text-decoration:underline"> ClickJacking </span>

### Task 6.7:

What version of php is the server using?
<br/>
Answer: <span style="text-decoration:underline"> 5.5.9-1ubuntu4.26 </span>
