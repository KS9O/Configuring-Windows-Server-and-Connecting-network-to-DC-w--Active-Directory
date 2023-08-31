# Configuring Windows Server and Network with Active Directory
## Table of Contents
1. Installation of Active Directory Doman Services

2. Promotion to Domain Controller

3. Adding non-GUI server to Domain

4. Joining non-GUI server to our GUI server

5. Adding Clients to the Domain

![Alt text](<assets/Domain Controller Dashboard.png>)
# Installation of Active Directory Domain Services
- After installation of our Windows Server 2016, I select the active directory domain services and added the proper features.
 ![Alt text](<Select Server role AD.png>)
![Alt text](<Active Directory installed-1.png>)

# Promoting to Domain Controller
- After AD DS installs we can promote to a DC
![Alt text](<Promote to Domain Controller.png>)
![Alt text](<domain controller options.png>)
- selecting a new forest, creating our root domain = cyber.local
![Alt text](<add a new forest called cyber.local.png>)
- With the NetBIOS = CYBER
- The server will restart and we successfully have installed ADDS and DNS on our microsoft windows 2016 server.
![Alt text](<after restart, we have our AD and DNS installed-1.png>)
# Joining our Non-GUI (Nano) Server to our DC
- In my nano server, entering the command : sconfig
- our nano server configuration opens up, selecting 1 to join our recently installed domain.
![Alt text](<Non-GUI interface.png>)
- We're promoted to restart the nano to add it to the domain
![Alt text](<joining non-gui to our domain cyber.local.png>)
# Joining Non-GUI Server to Domain Controller
- In our Server manage, we can pair our nano server to our cyber.local domain.
![Alt text](<Joining non-gui to DC.png>)
# Adding Clients to the Domain
- Creating our enterprise by adding clients to the server, i did this by pairing a windows 10 and windows 7 machine.
![Alt text](<adding clients10 ip  to domain.png>)
![Alt text](<adding clients7 ip to domain.png>)
- After adding both clients static IP's from the DNS server, using our cyber\administrator log in, i successfully add my windows 10 and windows 7 clients to our domain
![Alt text](<adding client 10 to domain.png>)
![Alt text](<adding client 7 to domain.png>)
- And here they are probably configured and connected to my DC.
![Alt text](<All our clients and servers in active directory.png>)