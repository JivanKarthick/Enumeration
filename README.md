# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.
Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

### site: 
This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com
## Output:
![image](https://github.com/JivanKarthick/Enumeration/assets/121165867/8d367d13-658f-42f3-a77a-ee87f0a0a827)



### filetype: 
This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
## Output:
![image](https://github.com/JivanKarthick/Enumeration/assets/121165867/cba271c6-26c4-41a5-83a8-515b01e5a1e2)





### intext: 
This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
## Output:
![image](https://github.com/JivanKarthick/Enumeration/assets/121165867/21ead395-f3c2-4a55-ae0c-5423b8253077)



### inurl: 
This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
## Ouput:
![image](https://github.com/JivanKarthick/Enumeration/assets/121165867/03cedb12-0d3d-4103-9829-e128976c42a8)



### intitle: 
This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
## Output:
![image](https://github.com/JivanKarthick/Enumeration/assets/121165867/41a43240-25ca-4e2e-8bde-2a2a607e8244)



### link: 
This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
## Output:
![image](https://github.com/JivanKarthick/Enumeration/assets/121165867/ad614b6b-e89c-48d0-a046-72de467e2fdb)



### cache: 
This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
## Output:
![image](https://github.com/JivanKarthick/Enumeration/assets/121165867/fddb6274-531d-452b-bb22-396d644a3e2c)


 
## DNS Enumeration


### DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

![image](https://github.com/JivanKarthick/Enumeration/assets/121165867/0e254d3e-fe8a-4b94-bac1-fbc8b09876f8)







## Dnsenum   
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.

![image](https://github.com/JivanKarthick/Enumeration/assets/121165867/d0801423-e0ad-4922-9774-249bcae7bd95)


## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
![image](https://github.com/JivanKarthick/Enumeration/assets/121165867/7bc3a67f-5318-44da-b977-be53bbce9e81)



In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
![image](https://github.com/JivanKarthick/Enumeration/assets/121165867/62acc2ae-4250-432b-bc6a-d92591f3040c)


select any username in the first column of the above file and check the same
![image](https://github.com/JivanKarthick/Enumeration/assets/121165867/3ee7a767-f6f4-4dc7-b946-2b71c8574c19)


## Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
## Output
  
![image](https://github.com/JivanKarthick/Enumeration/assets/121165867/4259cb5c-6b61-4857-81e7-06a4294b960c)



## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:

![image](https://github.com/JivanKarthick/Enumeration/assets/121165867/b812f1b2-329e-4ced-8d66-3c92401b01de)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully
