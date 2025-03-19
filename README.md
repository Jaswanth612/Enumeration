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

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain linkedin.com

![Screenshot 2025-03-15 132221](https://github.com/user-attachments/assets/fec4fd4c-f1e7-4c8b-96dd-926eccaa3fa2)

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain linkedin.com

![Screenshot 2025-03-15 132501](https://github.com/user-attachments/assets/14a417a6-a844-45c3-861a-5d17a7e4e099)



intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

![Screenshot 2025-03-15 132620](https://github.com/user-attachments/assets/2613eb42-7eb4-498c-a899-ffe9305d1353)




inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:Hafeezul" would search for pages that contain the word "admin" within the URL.

![Screenshot 2025-03-15 133009](https://github.com/user-attachments/assets/dbd57494-588d-4e5b-bf7d-a59cd092c1b2)



intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:Networkchuck of" would search for pages that contain "index of" within the title tag.

![Screenshot 2025-03-15 133102](https://github.com/user-attachments/assets/2e484432-8165-43b9-ad54-7b5222eb5171)





link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

![Screenshot 2025-03-15 133236](https://github.com/user-attachments/assets/92c2c616-1bc4-40c3-97c2-1cec2ef892b5)




cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

![Screenshot 2025-03-15 140513](https://github.com/user-attachments/assets/25a2fbe0-7911-4a92-a211-46b7a077d945)




 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

![Screenshot 2025-03-15 144134](https://github.com/user-attachments/assets/7f47110e-e603-4bad-9549-1ab12c4f9c22)







##dnsenum
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
##OUTPUT:

![Screenshot 2025-03-20 043136](https://github.com/user-attachments/assets/15d09d13-13c5-49dd-8013-2207ae06c131)


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
##OUTPUT:

![Screenshot 2025-03-20 043354](https://github.com/user-attachments/assets/40769c08-e995-4e0b-81a0-f8e51b158086)





In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:



select any username in the first column of the above file and check the same




#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands  
 
 ##Output
 
 ![Screenshot 2025-03-20 044246](https://github.com/user-attachments/assets/a2bff56c-144a-455d-a86f-aac26c5ba0b2)


  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

## OUTPUT:

![Screenshot 2025-03-20 044421](https://github.com/user-attachments/assets/4abfd1ce-e12a-4a00-8dae-b64d922036ad)



## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

