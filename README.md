<p align="center">
<img src="https://i.imgur.com/cO0oXGJ.jpg" height="20%" width="20%"/>
</p>

<h1 align="center">Virtual Private Networks (VPN) - Tunneling and IP Masking</h1>

<p>
This project demonstrates how a <b>Virtual Private Network (VPN)</b> changes network behavior by encrypting traffic and masking the client’s public IP address.
</p>

<p>
The objective is to understand how VPNs alter traffic routing, protect data in transit, and simulate different geographic locations.
</p>

<br />

<h2>Environment</h2>
<ul>
  <li>Microsoft Azure (Virtual Machine)</li>
  <li>Windows 10</li>
  <li>Remote Desktop</li>
  <li>Proton VPN</li>
  <li>Web Browser</li>
</ul>

<br />

<h2>Core Concepts</h2>
<ul>
  <li><b>Public IP Address</b> – Identifies a device on the internet</li>
  <li><b>VPN Tunnel</b> – Encrypted connection between client and VPN server</li>
  <li><b>IP Masking</b> – Replaces client IP with VPN server IP</li>
  <li><b>Traffic Routing</b> – Traffic is routed through VPN server instead of directly to destination</li>
</ul>

<br />

<h2>Baseline: Identifying Public IP</h2>

<p>
<ul>
  <li>Visit <b>https://whatismyipaddress.com</b> on your local machine</li>
  <li>Record your public IPv4 address</li>
</ul>
</p>

<br />

<h2>Creating a Virtual Machine</h2>

<p>
<ul>
  <li>Deploy a VM in Microsoft Azure</li>
  <li>Select a region different from your physical location</li>
  <li>Log into the VM via Remote Desktop</li>
  <li>Check public IP inside the VM</li>
  <li>The IP should differ from your local machine</li>
</ul>
</p>

<br />

<h2>Installing and Connecting to VPN</h2>

<p>
<ul>
  <li>Download and install <b>Proton VPN</b> on the VM</li>
  <li>Connect to a VPN server in a different region</li>
  <li>Check public IP again</li>
  <li>The IP now reflects the VPN server location</li>
</ul>
</p>

<br />

<h2>Observed Behavior Changes</h2>

<p>
<ul>
  <li>Public IP changes after VPN connection</li>
  <li>Traffic appears to originate from VPN server location</li>
  <li>Web content may adjust based on geographic region</li>
</ul>
</p>

<br />

<h2>Scenario</h2>
<ul>
  <li>A user connects to public Wi-Fi (untrusted network)</li>
  <li>VPN encrypts traffic before it leaves the device</li>
  <li>Traffic is routed through a secure VPN server</li>
  <li>Prevents interception and masks user identity</li>
</ul>

<br />

<h2>System Flow</h2>
<ul>
  <li>User initiates connection → VPN client encrypts traffic</li>
  <li>Traffic is sent through encrypted tunnel to VPN server</li>
  <li>VPN server forwards request to destination</li>
  <li>Destination sees VPN server IP, not client IP</li>
</ul>

<br />

<h2>Key Takeaways</h2>
<ul>
  <li>VPNs encrypt data in transit to protect against interception</li>
  <li>Public IP is replaced with the VPN server’s IP</li>
  <li>Traffic is rerouted through a secure intermediary</li>
  <li>VPNs improve privacy but do not replace endpoint security</li>
</ul>

<br />

<h2>What This Demonstrates</h2>
<ul>
  <li>Understanding of encrypted network tunneling</li>
  <li>Ability to validate IP masking and traffic redirection</li>
  <li>Awareness of network security in untrusted environments</li>
  <li>Practical use of VPNs in a cloud-based setup</li>
</ul>
