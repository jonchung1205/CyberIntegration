<h1> Failed RDP to Geoloacation Information </h1> 


<h2>Description</h2>
<b>The Powershell script in this repository is responsible for parsing out Windows Event Log information for failed RDP attacks and using a third party API to collect geographic information about the attackers location.
</b>
<br />
<br />
The script is used in this project where Azure Sentinel (SIEM) was configured and connected to a live virtual machine acting as a honey pot.
Throughout the span of the project, I was able to observe live attacks (RDP Brute Force) from across the world. A custom PowerShell script was used to
look up the attackers Geolocation information and it was plotted on an Azure Sentinel Map!
<br />
<br />

<p align="center">
<img src="https://github.com/jonchung1205/CyberIntegration/blob/main/images/API.png" height="85%" width="85%" alt="RDP event fail logs to iP Geographic information"/>
</p>
<h2>Languages Used</h2>
- <b>PowerShell:</b> Extract RDP failed logon logs from Windows Event Viewer 

<h2>Utilities Used</h2>

- <b>ipgeolocation.io:</b> IP Address to Geolocation API

<h2>Attacks coming in ; Custom logs being output with geodata</h2>

<p align="center">
<img src="https://github.com/jonchung1205/CyberIntegration/blob/main/images/CustomLogOutput.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>

<h2>World map of incoming attacks after 10 hours (built custom logs including geodata)</h2>

<p align="center">
<img src="https://github.com/jonchung1205/CyberIntegration/blob/main/images/Azure%20Cyber%20Map.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
