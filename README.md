This powershell script is used in 2 ways. This is designed to run remotely. it allows you to change the access control on programs and files. 

Line 1 defines $computers. You can either set it to a single machine or move line 3 to the end of line 1 so that it reads $Computers = Get-Content -path C:\Computers.txt. change the C:\computers.txt to wherever you have the linst of computer names. 
list a single computer per line.  

The next line test the connection to ensure the machine is online and reachable. 

Line 8 tells the script which program/file needs to be changed. it will grab the ACL for the file. 
line 9 changes the ACL. In this case we are changing the authenticated users deny write access. 
line 10 and 11 set the ACL. 
