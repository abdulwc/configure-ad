<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
In this project, I configured Active Directory services within the Azure cloud environment. This involved setting up a Domain Controller, managing user accounts, and establishing connectivity between client machines and the domain controller. Additionally, Remote Desktop access was enabled for non-administrative users to facilitate access to resources.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>Project Execution</h2>

<h3>Resource Setup in Azure</h3>

<p>
I initiated the project by creating the Domain Controller VM (named "DC-1") and the Client VM (named "Client-1") within the same Resource Group and Virtual Network. The Domain Controller's NIC was configured with a static IP address for consistent connectivity.
</p>


<br />

<h3>Connectivity Establishment</h3>

<p>
To ensure communication between the client and Domain Controller, I verified the placement of both VMs within the same Virtual Network using Azure Network Watcher. Connectivity was confirmed by successfully pinging DC-1’s private IP address from Client-1.
</p>


<br />

<h3>Active Directory Installation and Configuration</h3>

<p>
Active Directory Domain Services were installed on DC-1, which was subsequently promoted as a domain controller for the forest "mydomain.com." Administrative and normal user accounts were created and managed within Active Directory to facilitate access control and user management.
</p>


<br />

<h3>Domain Join and User Access Configuration</h3>

<p>
Client-1 was joined to the domain "mydomain.com," enabling centralized authentication and access control. Remote Desktop access was configured for non-administrative users, enhancing collaboration and resource accessibility.
</p>



<br />

<h3>User Account Management</h3>

<p>
Additional user accounts were created using a PowerShell script, demonstrating the scalability and efficiency of user management within Active Directory. User login functionality was verified on Client-1 to ensure access to domain resources.
</p>



<br />
<h2>Conclusion</h2>

<p>
This project showcases the successful configuration of Active Directory services in Azure, providing a robust identity and access management solution. By leveraging Azure infrastructure and Active Directory Domain Services, organizations can achieve greater efficiency, security, and scalability in managing user identities and access to resources within the cloud environment.
</p>

<br />
