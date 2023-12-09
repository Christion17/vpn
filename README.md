<p align="center">
<img src="https://i.imgur.com/cO0oXGJ.jpg" height = 20% width = 20%/>
</p>

<h1 align = "center">Understanding and Installing Virtual Private Networks</h1>
A Virtual Private Network (VPN) is a powerful security tool that connects two comptuers (networks) in a insecure network that is the Internet, allowing data to be encapsulated and encrypted between each other. This tutorial shows how to install a VPN through an Azure Virtual Machine environment (tutorial of how to set up VMs can be found <a href ="https://github.com/Christion17/vm-network">here</a>.

<br />

<h2>Environments and Technologies Used</h2>
<ul>
  <li>Microsoft Azure (Virtual Machines/Compute)</li>
  <li>Remote Desktop</li>
  <li>Internet Browser of your choice</li>
  <li>Proton VPN</li>
  <li>Notepad to type down IP Addresses</li>
</ul>

<br />

<h2>Operating Systems Used</h2>
<ul>
  <li>Windows 10 Pro (21H2)</li>
</ul>

<br />

<h2>Installing Proton VPN</h2>

<h3>Setting up Resources and Citing IP Addresses</h3>

<p>
  <ul>
    <li>Before setting up, browse to <a href ="https://whatismyipaddress.com/">What Is My IP Address</a> and take note of your IPv4 Address</li>
    <li>Now go to the Microsoft Azure Portal and create a Resource Group and a Virtual Machine. When creating your VM, make sure the <b>Region</b> is set in a region outside of your country</li>
    <li>Log in to your VM through Remote Desktop and go to What Is My IP Address. The IPv4 Address in the VM should be <b>different</b> than the one on your main computer.</li>
  </ul>
</p>

<br />

<h3>Signing up and configuring Proton VPN</h3>

<p>
  <ul>
    <li>Sign up for a free version of <a href ="https://account.protonvpn.com/signup?plan=free&language=en">Proton VPN</a></li>
    <li>Head back to your VM, download the Proton VPN client</li>
    <li>After installing, log in to Proton VPN and choose a VPN server to connect to outside of your VM's region</li>
    <li>After connecting to a VPN Server, go to What Is My IP Address and notice the IPv4 Address is different</li>
    <li>Attempt to browse websites such as Google or Amazon and notice the differences related to  your VPN Server (such as seeing Hangul is connected to a VPN server in South Korea)</li>
  </ul>
</p>

<br />
