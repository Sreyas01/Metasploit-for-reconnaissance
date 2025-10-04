# Metasploit-for-reconnaissance
## NAME:Ashwin Kumar A
## REGISTER NUMBER:212223040021
# Metasploit
Metasploit for reconnaissance in pentesting

# AIM:

To get introduced to Metasploit Framework and to  perform reconnaissance  in pentesting .

## DESIGN STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various categories of tools as follows:

### Step 3:

Open terminal and try execute some kali linux commands

## EXECUTION STEPS AND ITS OUTPUT:

Find out the ip address of the attackers system
## OUTPUT:

<img width="635" height="347" alt="image" src="https://github.com/user-attachments/assets/2e76e8d5-6a78-49d0-84a4-1f255b8d0b9c" />

Invoke msfconsole:
## OUTPUT:

<img width="677" height="820" alt="image" src="https://github.com/user-attachments/assets/6091c181-ad48-49fb-8809-e4950f6d547a" />


Type help or a question mark "?" or help to see the list of all available commands you can use inside msfconsole.
## OUTPUT:

<img width="750" height="675" alt="image" src="https://github.com/user-attachments/assets/e07a7616-2f93-47d8-a20d-1eac49d7c7a2" />

Port Scanning:
Following command is executed for scanning the systems on our local area network with a TCP scan (-sT) looking for open ports between 1 and 1000 (-p1-1000).
msf >  nmap -sT 192.168.56.101/24 -p-1000

## OUTPUT:

<img width="619" height="297" alt="Screenshot 2025-09-30 113056" src="https://github.com/user-attachments/assets/bf5ee210-b7a0-421e-90b3-74901bb250ae" />

use the db-nmap command to scan and save the results into Metasploit's postgresql attached database. In that way, you can use those results in the exploitation stage later.
scan the targets with the command db_nmap as follows.
msf > db_nmap 192.168.56.101/24

## OUTPUT:

<img width="639" height="265" alt="Screenshot 2025-09-30 113920" src="https://github.com/user-attachments/assets/19c23eaa-a733-4af6-8512-31d945ae5e52" />


Search is a powerful command in Metasploit that you can use to find what you want to locate. 
msf >search name:Microsoft type:exploit
## OUTPUT:

<img width="642" height="560" alt="image" src="https://github.com/user-attachments/assets/779572b6-66d6-4248-b611-1d83bb998053" />

The info command provides information regarding a module or platform,
## OUTPUT:

<img width="1095" height="563" alt="image" src="https://github.com/user-attachments/assets/17817e9a-b9c1-4284-9447-8f2452141fdd" />


## MYSQL ENUMERATION
Find the IP address of the Metasploitable machine first. Then, use the db_nmap command in msfconsole with Nmap flags to scan the MySQL database at 3306 port.
db_nmap -sV -sC -p 3306 <metasploitable_ip_address>
## OUTPUT:

<img width="862" height="153" alt="image" src="https://github.com/user-attachments/assets/fbd0729e-1271-4f8d-a815-d88f1db61ff8" />

Use the search option to look for an auxiliary module to scan and enumerate the MySQL database.
search type:auxiliary mysql
## OUTPUT:

<img width="1098" height="472" alt="image" src="https://github.com/user-attachments/assets/3d94e5ad-0612-45b3-bc34-642615d3ed30" />


use the auxiliary/scanner/mysql/mysql_version module by typing the module name or associated number to scan MySQL version details.
use 11
Or:
use auxiliary/scanner/mysql/mysql_version
## OUTPUT:
<img width="1088" height="427" alt="image" src="https://github.com/user-attachments/assets/6fa9b14f-a23c-4467-b785-bc668bc184d5" />


Use the set rhosts command to set the parameter and run the module, as follows:
## OUTPUT:
<img width="724" height="289" alt="image" src="https://github.com/user-attachments/assets/6dc2dad7-2b66-4dfd-a2d0-9e6861984147" />

After scanning, you can also brute force MySQL root account via Metasploit's auxiliary(scanner/mysql/mysql_login) module.
## OUTPUT:

<img width="724" height="289" alt="Screenshot 2025-09-30 091328" src="https://github.com/user-attachments/assets/6ff2fe3b-b903-4764-ac04-185d6f08140c" />

set the PASS_FILE parameter to the wordlist path available inside /usr/share/wordlists:
set PASS_FILE /usr/share/wordlistss/rockyou.txt
Then, specify the IP address of the target machine with the RHOSTS command.
set RHOSTS <metasploitable-ip-address>
Set BLANK_PASSWORDS to true in case there is no password set for the root account.
set BLANK_PASSWORDS true
## OUTPUT:
<img width="1105" height="307" alt="Screenshot 2025-09-29 113341" src="https://github.com/user-attachments/assets/6f8b6b1f-c868-4f75-b53a-65b0f76b5371" />


## RESULT:
The Metasploit framework for reconnaissance is  examined successfully
