# CCNA SSH Implementation

\>en  
\#conf t  
fig#hostname R1  
fig#int g#/#  
if#ip add (ip address) (subnetmask)  
if#no shut  
if#exit  
fig#ip domain-name name.com  
fig#crypto generate rsa  
(pick a number between 1024 or 2048 though 1024 is suffecient)  
fig#ip ssh v 2  
fig#ip ssh time 60 (60 seconds before sission expires)  
fig#ip ssh auth 3 (3 tries)  
fig#line vty 0 4  
line#transport input ssh  
line#login local  
line#end  
\#copy run star  

-------------------------------  
for troubleshooting use:  
\#show ssh  
\#show ip ssh  
\#show session  
\#show users  
\#show running-config | section line vty  
\#depending on what you need  
