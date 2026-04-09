# Task 4 – Exploitation & System Security

## Objective
To understand how attackers gain access to vulnerable systems and analyze security weaknesses.

## Tools Used
- Nmap
- SSH

## Steps Performed

1. Identified target system using network scanning.
2. Discovered open services on the target machine.
3. Attempted exploitation using Metasploit (unsuccessful due to configuration constraints).
4. Gained access to the system using default credentials via SSH.
5. Executed basic commands to verify access.

## Commands Used

nmap -sn 192.168.56.0/24  
nmap -sV 192.168.56.101  
ssh -oHostKeyAlgorithms=+ssh-rsa -oKexAlgorithms=+diffie-hellman-group1-sha1 msfadmin@192.168.56.101  
whoami  
uname -a  

## Outcome
Successfully accessed the target system using weak credentials, demonstrating a common security vulnerability.

## Conclusion
This task highlights the importance of:
- Strong authentication mechanisms
- Disabling default credentials
- Keeping systems updated

Understanding these vulnerabilities helps in securing systems against real-world attacks.
