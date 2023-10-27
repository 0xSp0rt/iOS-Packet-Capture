<h1>iOS Packet Capture</h1>

<h2>Description</h2>
This project provides a walkthrough on how to capture and analyze network traffic on ios devices with wireshark using Xcode. Xcode is a software development tool built by Apple inc for apple devices, the Xcode application allows us to run the Remote virtual interface tool(rvictl) command which allows us to create an interface that allows us to capture the network traffic from the iOS device on wireshark. It is important to acquire the UDID of the device to be captured as it will be used in terminal to run the command.
<br />


<h2>Utilities Used</h2>

- <b>Xcode</b> 
- <b>Wireshark</b>
- <B>Terminal</b>

<h2>Environments Used </h2>

- <b>MacOS Sonoma</b>
- <b>iOS 17.0.3

<h2>Program walk-through:</h2>

<p align="center">
Go to the app store and download Xcode: <br/>
<img src="https://imgur.com/bVxbMpo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Plug in the device with a usb and allow trust, open xcode and click on the windows menu > device and simulators > connected devices then copy the identifier(UDID):  <br/>
<img src="https://imgur.com/u7c7U2I.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Open terminal and run the command "ifconfig -l" to check the preexisting network interfaces: <br/>
<img src="https://imgur.com/atETaiH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
