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
Select the disk:  <br/>
<img src="https://i.imgur.com/tcTyMUE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter the number of passes: <br/>
<img src="https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
