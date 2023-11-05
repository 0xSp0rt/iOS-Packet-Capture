<h1>iOS Packet Capture</h1>

<h2>Description</h2>
This project provides a walkthrough on how to capture and analyze network traffic on ios devices with wireshark using Xcode. Xcode is a software development tool built by Apple inc for apple devices, the Xcode application allows us to run the Remote virtual interface tool(rvictl) command which allows us to create an interface that allows us to capture and analyze the network traffic from the iOS device on wireshark. Capturing live packets from these devices can aid digital forensics, investigate security threats and also aid network troubleshooting. It is important to acquire the UDID of the device to be captured as it will be used in terminal to run the command required to create the network interface.
<br />


<h2>Utilities Used</h2>

- <b>Xcode</b> 
- <b>Terminal</b>
- <B>Wireshark</b>

<h2>Environments Used </h2>

- <b>MacOS Sonoma</b>
- <b>iOS 17.0.3

<h2>Project walk-through:</h2>

<p align="center">
Go to the app store and download Xcode: <br/>
<img src="https://imgur.com/bVxbMpo.png" height="80%" width="80%" alt="iOS Packet Capture"/>
<br />
<br />
Plug in the device with a usb and allow trust, open xcode and click on the windows menu > device and simulators > connected devices then copy the identifier(UDID). It is important to note that an hypen should be placed after the first 8 digits of the UDID to enable the remote virtual interface run the command in terminal:  <br/>
<img src="https://imgur.com/u7c7U2I.png" height="80%" width="80%" alt="iOS Packet Capture"/>
<br />
<br />
Open terminal and run the command "ifconfig -l" to check the preexisting network interfaces: <br/>
<img src="https://imgur.com/nO8SuBm.png" height="80%" width="80%" alt="iOS Packet Capture"/>
<br />
<br />
Run the command "rvictl -s UDID", this allows us to create the network interface to analyze and capture the iOS device packets:  <br/>
<img src="https://imgur.com/Da1sHnP.png" height="80%" width="80%" alt="iOS Packet Capture"/>
<br />
<br />
Run the command "ifconfig -l" to confirm the interface has been added, observe below that the interface "rvi0" has been added:  <br/>
<img src="https://imgur.com/7QYmZLg.png" height="80%" width="80%" alt="iOS Packet Capture"/>
<br />
<br />
Open wireshark and observe the interface "rvi0" has been added to capture network traffic:  <br/>
<img src="https://imgur.com/6NB5z9l.png" height="80%" width="80%" alt="iOS Packet Capture"/>
<br />
<br />
Click on the rvi0 interface to start packet capture as shown below:  <br/>
<img src="https://imgur.com/qODeNr2.png" height="80%" width="80%" alt="iOS Packet Capture"/>
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
