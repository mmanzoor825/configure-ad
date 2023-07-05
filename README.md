<p align="center">
  <img width="600" height="300" src="https://github.com/mmanzoor825/configure-ad/assets/138532574/f0104599-f417-42c5-a46f-b09e07e0a7f7">
</p>

<h1>Active Directory - Installation and configuration</h1>
This tutorial outlines the installation of Microsoft Active Directory.<br />

<h2>Environments and Technologies Used</h2>

- Oracle VM VirtualBox

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 Pro</b> 

<h2>Installation Steps</h2>

<p>
  <img width="585" alt="image" src="https://github.com/mmanzoor825/configure-ad/assets/138532574/98f403ed-cf25-4623-a1de-ebb1922d9694">
>

</p>
<p>
To install Active Directory on the server, go to Server Manager > Add roles and features > click next > choose "Role-based or feature-based installation" > Select a server from the server pool > Choose Active Directory Domain Services and click add features. Click next until the confirmation page and select install.  </p>

</p>
<br />

<p>
<img width="280" alt="image" src="https://github.com/mmanzoor825/configure-ad/assets/138532574/4d214270-c6c4-4479-ab13-e3a5c74f5fdf">

</p>
<p>
Now we need to promote the server to a domain controller. Do this by clicking the notifications icon at the top right and click "Promote this server to domain controller". Choose "Add a new Forest" and create a Root domain name (ex. mydomain.com). Create a restore password. Click next until the prerequisites check page and click install. The computer will restart.
                                                                                                                                                        
</p>
<br />

<p>
<img width="325" alt="image" src="https://github.com/mmanzoor825/configure-ad/assets/138532574/0d389d0f-63a0-42d5-911a-275f7fff40b5">
</p>
<p>
Now lets create a user in the domain. Go to Tools > Active Directory Users and Computers. Right click your domain and select new > User. Follow the instructions and create a new user.  </p>
<br />

<p>
<img width="241" alt="image" src="https://github.com/mmanzoor825/configure-ad/assets/138532574/b186c98f-0ad1-442b-9568-b7c6d51b37b5">

Now we will add a separate user computer on the network to the domain. First assign the server a static IP address. Then we have to change the DNS server of the client machine to the IP address of the server. Next go to file explorer and right-click This PC. Click properties and scroll down to "Rename this PC (advanced)". Click change and type the name of the domain. Next you will be prompted to enter valid credentials to enter the domain. Restart will be required.
</p>
<br />

<p>



<br />
