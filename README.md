<h1>Active Directory & Windows Server Lab</h1>

<h2>Overview</h2>
A guided personal lab, completed in late 2023, that builds a small Active Directory environment in Oracle VirtualBox. It is a learning project on a personal computer, not production work.

<b>What it covers:</b>

- Installing Windows Server on a virtual machine and promoting it to a domain controller with Active Directory
- Creating a domain and assigning an IPv4 address on an internal network
- Configuring NAT and routing (Remote Access) so clients on the internal network can reach the internet through the domain controller
- Installing DHCP and setting a scope so client machines receive IP addresses automatically
- Running an existing PowerShell script to create 1,000 user accounts in Active Directory (I executed the script; I did not write it)
- Creating a second virtual machine (CLIENT1) and joining it to the domain

<h2>Tools and Environment</h2>

- <b>Oracle VirtualBox</b> (virtualization), on a Windows 10 host PC
- <b>Windows Server</b> (evaluation ISO) as the domain controller
- <b>Windows client VM</b> (CLIENT1) joined to the domain
- <b>PowerShell</b> (running the existing user-creation script)

<h2>Walk-through</h2>

<p align="center">
Download Oracle VirtualBox and install Windows Server on the first virtual machine (the domain controller): <br/>
<img src="https://imgur.com/jGnqwdC.png" height="80%" width="80%" alt="VirtualBox manager and Windows Server setup on the domain controller VM"/>
<br />
<br />
Rename the network adapters for home internet and the internal network: <br/>
<img src="https://imgur.com/JbOd4ia.png" height="80%" width="80%" alt="Renamed network adapters on the domain controller"/>
<br />
<br />
Assign an IP address on the internal network: <br/>
<img src="https://imgur.com/nyTHVhs.png" height="80%" width="80%" alt="IP address settings for the internal network adapter"/>
<br />
<br />
Install Active Directory on the domain controller:  <br/>
<img src="https://imgur.com/l7taOvZ.png" height="80%" width="80%" alt="Installing Active Directory Domain Services"/>
<br />
<br />
Create the domain:  <br/>
<img src="https://imgur.com/3GVmaLW.png" height="80%" width="80%" alt="Creating the Active Directory domain"/>
<br />
<br />
Install Remote Access and configure NAT and routing so clients on the internal network can reach the internet through the domain controller:  <br/>
<img src="https://imgur.com/FdNXxIw.png" height="80%" width="80%" alt="Installing the Remote Access role"/>
<br />
<br />
Routing and Remote Access setup wizard with NAT selected: <br/>
<img src="https://imgur.com/YsRJwO2.png" height="80%" width="80%" alt="Routing and Remote Access setup wizard with NAT selected"/>
<br />
<br />
Install DHCP and set a DHCP scope on the domain controller so client computers get an IP address automatically:  <br/>
<img src="https://imgur.com/YWEW3te.png" height="80%" width="80%" alt="Installing DHCP and creating a scope"/>
<br />
<br />
Run the existing PowerShell script to create users in Active Directory: <br/>
<img src="https://imgur.com/pRJwIlX.png" height="80%" width="80%" alt="Running the PowerShell user-creation script"/>
<br />
<br />
<img src="https://imgur.com/lKBrWxQ.png" height="80%" width="80%" alt="PowerShell script run, continued"/>
<br />
<br />
Create a second virtual machine (CLIENT1) on the internal network and join it to the domain:  <br/>
<img src="https://imgur.com/7qmVmAA.png" height="80%" width="80%" alt="Creating the CLIENT1 virtual machine and joining it to the domain"/>
<br />
<br />
DHCP lease and the CLIENT1 computer account in Active Directory Users and Computers: <br/>
<img src="https://imgur.com/z9bIrnR.png" height="80%" width="80%" alt="DHCP address lease and CLIENT1 computer account in Active Directory"/>
</p>
