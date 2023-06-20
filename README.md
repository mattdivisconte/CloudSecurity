# Cloud Security

<h2>Description</h2>
For this project, we needed to create a secure Azure Cloud setup for a RedTeam penetration test

<h3>Virtual Network Diagram</h3>

Network Diagram:  <br/>
<img src="https://i.imgur.com/lnW9XWG.jpg" height="80%" width="80%" alt="Network Diagram"/>
<br />

<h3>Steps Taken:</h3>
1. Create a Resource Group (RedTeamAzure)</br>
2. Create Virtual Network (VNet)</br>
3. Create a Network Security Group (NSG)</br>
4. Create an NSG Rule to Deny All Inbound/Outbound Traffic</br>
5. Create a Virtual Jumpbox Provisioner (SSH Only Access)</br>
6. Create three Virtual Web Servers (SSH Only Access)</br>
7. Create an Inbound NSG rule to allow SSH on port 22 from my home IP address to the Jumpbox</br>
8. Install Docker</br>
9. Pull Ansible container</br>
10. Create NSG rule to allow SSH from JumpBox IP to virtual network</br>
11. Run Ansible container and connect to it</br>
12. Generate SSH key from container and overwrite Web Server SSH access key with Ansible VM key</br>
13. Configure Ansible to connect to the Web Servers</br>
14. Run Ansible Playbook to install DVWA on the Web Server</br>
15. Create a Load Balancer with a front end public IP address and the backend connected to the Web Servers</br>
16. Create a Load Balancing Rule to forward port 80 to the Web Servers allowing session persistence</br>
17. Create an NSG rule to allow external internet traffic on port 80 from my home IP address to the load balancer and VNet</br>
18. Test load balancer by connecting to and then shutting off various Web Servers</br>
<br></br>


