<h1>Home-Lab-Attack-Analyze</h1>

 ### [YouTube Demonstration](https://youtu.be/7eJexJVCqJo)

<h2>Description</h2>
Designed a homelab with two virtual machines: an attacker machine(Kali Linux) and a defender machine (Windows with Splunk as the SIEM). Developed a custom malware payload disguised as "CV.pdf.exe" using Kali Linux, performed port scanning with nmap and successfully executed remote commands on the Windows machine. Monitored the attack using Sysmon and Splunk analyzing the malicious activity and identifying indicators of compromise. Mapped observed techniques to the MITRE ATT&CK framework and strategies to enhance the defense mechanisms<br />


<h2>Environments Used </h2>

- <b>VMWare</b> (21H2)
- <b>Windows 10 media tool</b> (21H2)
- <b>Kali Linux</b> (21H2)
- <b>Splunk</b> (21H2)
  
<h2>Project walk-through:</h2>

<p align="center">
Launch the WMare: <br/>
<img src="https://i.imgur.com/BefFlTC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
 <img src="https://i.imgur.com/Yb3lVBl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Create Malware using Kali Linux:  <br/>
<img src="https://i.imgur.com/LSeHVZP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Set up handler to start listening from Attacker machine: <br/>
<img src="https://i.imgur.com/rGNuLUJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
This will allow the person on the end of the target machine to download the malware from the attacker:  <br/>
<img src="https://i.imgur.com/0OCGmLU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Download Malware:  <br/>
<img src="https://i.imgur.com/7vb57TR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Open windows shell from Kali:  <br/>
<img src="https://i.imgur.com/J3rxXie.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Run Commands:  <br/>
<img src="https://i.imgur.com/XKmzA2l.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<img src="https://i.imgur.com/XKmzA2l.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
 <img src="https://i.imgur.com/or37ICu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
 Go to windows,Open Splunk and start searching the endpoint for the malware saved as CV.pdf.exe:  <br/>
<img src="https://i.imgur.com/O5MVIZW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
 Expand the results and copy the process id:  <br/>
<img src="https://i.imgur.com/oOJbS7Q.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
 Search using the process id to do some telementry.The command lines used are revealed and technique id:  <br/>
 <img src="https://i.imgur.com/LgBRmnK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
