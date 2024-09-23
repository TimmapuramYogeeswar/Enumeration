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
Following searches for all the sites that is in the domain yahoo.com

OUTPUT

![image](https://github.com/user-attachments/assets/d2aa7393-bc08-4f04-9c5c-44a5a51205bc)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

OUTPUT

![image](https://github.com/user-attachments/assets/f9b2240f-6e3e-4746-a559-2f64da77bbe6)




intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

OUTPUT

![image](https://github.com/user-attachments/assets/f9c8695b-763b-4577-9ca2-aad0514cf4ba)


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

OUTPUT

![image](https://github.com/user-attachments/assets/f338b96f-30b5-4d82-9f9e-0495a07483e0)


intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

OUTPUT

![image](https://github.com/user-attachments/assets/2a21dc75-cbfd-48e7-a9d0-402618e9efeb)


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

OUTPUT

![image](https://github.com/user-attachments/assets/91c766b5-d910-4ea6-b463-6ef7c5c40d51)


cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

OUTPUT

![image](https://github.com/user-attachments/assets/ae9b1ad6-769a-48d1-b800-0423ec7d2ecd)

 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion

OUTPUT

![image](https://github.com/user-attachments/assets/cc1404d1-6d87-48f2-a279-666fe37cf107)

## OUTPUT:

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

OUTPUT

![image](https://github.com/user-attachments/assets/445d393b-0776-4e03-8f60-d46dbc5b5b2d)


![image](https://github.com/user-attachments/assets/23e382fe-3b18-4d6a-aa22-a5a32ad296a5)


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

OUTPUT

![image](https://github.com/user-attachments/assets/370f3ab4-c247-4de5-875f-3fef91fd36ea)


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
select any username in the first column of the above file and check the same

OUTPUT

![image](https://github.com/user-attachments/assets/1974ac43-de34-452a-a581-60912fe0bdae)


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ##Output
  
![image](https://github.com/user-attachments/assets/50312589-5083-4a6e-a528-c9f9d6dfc40b)


## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:

![image](https://github.com/user-attachments/assets/55fe9106-c4cb-43ee-9b9c-eeea17dfea5d)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

