# Metasploit-for-reconnaissance
# Metasploit
Metasploit for reconnaissance in pentestin

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

 Identify the Attacker’s IP Address
Determine the IP address of the attacker's system.

## OUTPUT

![image](https://github.com/user-attachments/assets/14f8e813-d318-43ff-b3f8-ce63459d1db9)

 Launch the Metasploit Console
Invoke the msfconsole.

## OUTPUT:

![image](https://github.com/user-attachments/assets/4ddd41f8-4697-4dde-8536-b81191afe255)

To view available commands, enter "?".


![image](https://github.com/user-attachments/assets/7ed82e4f-6c0f-43cd-aedb-44dfeef23b17)

 Generate Payload Using msfvenom
Execute the following command to generate a Windows Meterpreter reverse shell payload.

 Set Up an HTTP Server
Once the payload file is created, navigate to the home directory. Right-click and select "Open Terminal Here."

Run the Python command to establish an HTTP server for file distribution.

![image](https://github.com/user-attachments/assets/bb87ab0f-a3b9-4c0d-b2a2-e1d893929c91)

Distribute the Payload
Share the .exe file with the target system via any medium or the HTTP server. Once the victim downloads and executes the file, the exploit is triggered.

 VICTIM DEVICE:
 Establish a Connection
On Kali Linux, reopen the terminal and invoke msfconsole. Follow the necessary steps to establish a connection with the victim’s device.

![image](https://github.com/user-attachments/assets/16713749-6505-4197-871b-eeb3b2d95302)

Once exploited, a session is created, allowing remote access without the victim’s awareness.

 Execute Commands on the Victim’s Device
Use the help command to list available operations.

![image](https://github.com/user-attachments/assets/4a41c049-9b7a-4430-a9b5-d8a52e696afd)



## RESULT:
The Metasploit framework for reconnaissance is examined successfully.
