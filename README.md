<h1>Network Home Lab</h1>



<h2>Description</h2>
In this home lab we're going to walk through how to configure a basic network using Cisco Packet Tracer. Configuring an running this lab will help develop your understanding of how networking works, so I'd highly recommend running through it a couple times. Please ask questions where any part becomes unclear, and eventually try to build it on your own.
<br />


<h2>Devices and Connections Used:</h2>

- <b>PC(4)</b> 
- <b>Switches(2)</b>
- <b>Router(1)</b>
- <b>Copper Straight-Throught(6)</b>

<h2>Environments Used </h2>

- <b>MacOS</b> 

<h2>Program walk-through:</h2>


Create Our Topology: <br/>
<img src="https://i.imgur.com/sXjcBVM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br />
<br />


Use the Copper Straight-Through cable to connect PC0 and PC1 to Switch0(using FastEthernet0) : <br/>
<img src="https://i.imgur.com/Ijs6xXG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />


Connect Switch0 to PC0 and PC1(using FastEthernet0/1 and FastEthernet0/2) : <br/>
<img src="https://i.imgur.com/Ijs6xXG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/tpIZGih.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br />
<br />


Connect PC2 and PC3 to Switch1(using FastEthernet0 to FastEthernet0/1) <br/>
<img src="https://i.imgur.com/OpAwnkM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br />
<br />

Connect PC2 and PC3 to Switch1(using FastEthernet0 to FastEthernet0/2) <br/>
<img src="https://i.imgur.com/SrID0Y1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br />
<br />

Connect Switch1 to PC2 and PC3(using FastEthernet0/1 to FastEthernet0/2) : <br/>
<img src="https://i.imgur.com/MYPfl08.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/SrID0Y1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br />
<br />

With a Copper Straight-Through cable connect Switch0 to the Router(using GigabitEthernet0/1 to GigabitEthernet0/0) <br/>
<img src="https://i.imgur.com/GPaxBBO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/9UUA0sY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<br />
<br />
With a Copper Straight-Through cable connect Switch0 to the Router(using GigabitEthernet0/1 to GigabitEthernet0/0) <br/>
<img src="https://i.imgur.com/GPaxBBO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/9UUA0sY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<br />
<br />

- <b>Double click your newly created VM</b> 
- <b>Choose the virtual optical disk file and select the server that youve downloaded(sever2019 iso)</b>
- <b>After installation is complete, you must complete the windows setup</b>
- <b> Once complete, You will be prompt to create a administration account.(enter a password)</br>
<br />
<br />
Set up Internal IP address:<br />
- <b> Navigate to the network icon at the bottom right of your screen</br>
- <b>Click network<br />
- <b>Click change adapter options<br />
- <b> Name your networks(Internet & Internal)<br />
- <b> To figure out which network Internet & which is the Internal right click and select properties. <br />
- <b> Now you must give the internal network an ip address. <br />
- <b> right click the internal network and select properties<br />
- <b> Click Internet Protocal Version 4(TCP/IPv4) <br />
- <b> Assign a IP address(172.16.0.1) and subnet mask(255.255.255.0) <br />
- <b> For the preferred DNS server enter its IP address(172.16.0.1) <br />
<img src="https://i.imgur.com/LT7cdsg.png?1" height="80%" width="80%" alt="Disk Sanitization Steps"/>


Install Active Directory Domain Serves: <br />
- <b> Navigate to server manager dashboard by clicking on the start menu then clicking server manager </br>
- <b> Click add roles and features</br>
<img src="https://i.imgur.com/fOYce8T.png?1" height="80%" width="80%" alt="Disk Sanitization Steps"/>

- <b> Pick the server you want to install</br>
<img src="https://i.imgur.com/KZpRXWn.png?1" height="80%" width="80%" alt="Disk Sanitization Steps"/>





 Rename this PC: <br />
  - <b> Right click the start menu and click system<br />
   - <b> Click rename this PC<br />
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
