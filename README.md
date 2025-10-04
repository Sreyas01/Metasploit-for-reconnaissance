# Metasploit-for-reconnaissance

# Metasploit

Metasploit for reconnaissance in pentesting

## AIM:

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

### OUTPUT:

<img width="761" height="439" alt="image" src="https://github.com/user-attachments/assets/4c86d131-03c8-44e1-b03d-d58c3aa66ccb" />

## Invoke msfconsole

### OUTPUT:

<img width="602" height="527" alt="image" src="https://github.com/user-attachments/assets/15e28d9c-25e7-4909-9974-3722fdaaf1ff" />

Type help or a question mark "?" to see the list of all available commands you can use inside msfconsole.

<img width="684" height="867" alt="image" src="https://github.com/user-attachments/assets/36003a67-4191-4ca2-a8b9-4bff5303b79d" />

## Port scanning:

### msf > nmap -sT 192.168.1810/24-p1-1000

<img width="734" height="418" alt="image" src="https://github.com/user-attachments/assets/e871d329-fc68-42c2-825d-5c84f8410e34" />

### msf > db_nmap 192.168.181.0/24

<img width="825" height="345" alt="image" src="https://github.com/user-attachments/assets/189142ad-6815-4dc3-8db0-1f093346f637" />

### kali > ls-l

<img width="516" height="89" alt="image" src="https://github.com/user-attachments/assets/199c5add-5d60-4748-ae17-52075a6c70e3" />

### search 


### info

<img width="826" height="766" alt="image" src="https://github.com/user-attachments/assets/b7f74d3b-adf5-4fb5-a9e3-3bce5796fe3e" />

## MYSQL ENUMERATION

### db_nmap -sV -sC -p 3306 <metasploitable_ip_address>

<img width="825" height="345" alt="image" src="https://github.com/user-attachments/assets/a6398b67-257e-40c3-8634-7afbb3cb8a77" />

### search

<img width="824" height="223" alt="image" src="https://github.com/user-attachments/assets/06568ffd-094e-4244-b166-82970e4d17bb" />

###  use 11 Or: use auxiliary/scanner/mysql/mysql_version

<img width="818" height="158" alt="image" src="https://github.com/user-attachments/assets/66b252ea-3514-44f1-a550-7fa89fa31507" />

### Use the set rhosts command to set the parameter and run the module, as follows:

<img width="823" height="111" alt="image" src="https://github.com/user-attachments/assets/eaff8658-4245-4087-9462-f70338bf7e8a" />

### After scanning, you can also brute force MySQL root account via Metasploit's auxiliary(scanner/mysql/mysql_login) module.

<img width="826" height="309" alt="image" src="https://github.com/user-attachments/assets/34b5c4d4-37d6-43f0-8a9a-70c38a21ff7a" />

### /usr/share/wordlists: set PASS_FILE /usr/share/wordlistss/rockyou.txt 

<img width="826" height="311" alt="image" src="https://github.com/user-attachments/assets/8a5e2345-fb27-40f2-acba-2215a8fd6c3e" />

<img width="820" height="230" alt="image" src="https://github.com/user-attachments/assets/217fbd68-9d4b-4bdb-b693-8c812d2f16db" />

## RESULT:
The Metasploit framework for reconnaissance is  examined successfully
