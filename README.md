<h1>Home-Lab-Attack-Analyze</h1>

 ### [YouTube Demonstration](https://youtu.be/7eJexJVCqJo)

<h2>Description</h2>
Designed a homelab with two virtual machines: an attacker machine(Kali Linux) and a defender machine (Windows with Splunk as the SIEM). Developed a custom malware payload disguised as "CV.pdf.exe" using Kali Linux, performed port scanning with nmap and successfully executed remote commands on the Windows machine. Monitored the attack using Sysmon and Splunk analyzing the malicious activity and identifying indicators of compromise. Mapped observed techniques to the MITRE ATT&CK framework and strategies to enhance the defense mechanisms<br />


<h2>Environments Used </h2>

- <b>VMWare</b> 
- <b>Windows 10 media tool</b> 
- <b>Kali Linux</b> 
- <b>Splunk</b> 
  
<h2>Project walk-through:</h2>

<p align="center">
 <h3>Launch the WMare:</h3> <br/>
<img src="https://i.imgur.com/BefFlTC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
  <img src="https://i.imgur.com/Yb3lVBl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 <h3>Create payload Malware on Kali using this command: </h3> <br/>
<img src="https://i.imgur.com/LSeHVZP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 <h3>Set up handler to start listening from Attacker machine:</h3> <br/>
<img src="https://i.imgur.com/rGNuLUJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 <h3>This will allow the person on the end of the target machine to download the malware from the attacker: </h3> <br/>
<img src="https://i.imgur.com/0OCGmLU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 <h3>Download Malware from the Windows machine:</h3>  <br/>
<img src="https://i.imgur.com/7vb57TR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 <h3>Once the RDP(Remote Desktop Protocol) connection is setup, Open the shell to start running commands:</h3>  <br/>
<img src="https://i.imgur.com/J3rxXie.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 <h3>Run Commands: </h3> <br/>
<img src="https://i.imgur.com/XKmzA2l.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<img src="https://i.imgur.com/XKmzA2l.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
  <h3>The IP address returned is that of the target machine:</h3>  <br/>
 <img src="https://i.imgur.com/or37ICu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

 <h2>SIEM Analyses:</h2>

 <p align="center">
  <h3>Go to windows,Open Splunk and start searching the endpoint for the malware saved as CV.pdf.exe:</h3>  <br/>
<img src="https://i.imgur.com/O5MVIZW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 <h3> Expand the results and copy the process id: </h3> <br/>
<img src="https://i.imgur.com/oOJbS7Q.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
  <h3>Search using the process id to do some telementry.The command lines used are revealed and technique id: </h3> <br/>
 <img src="https://i.imgur.com/LgBRmnK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
  <h3>Attack Techniques revealed:</h3>  <br/>
 <img src="https://i.imgur.com/tTcEQtX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />  
<img src="https://i.imgur.com/3mwAM8t.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />  
<img src="https://i.imgur.com/AmqmpzA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />  
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
