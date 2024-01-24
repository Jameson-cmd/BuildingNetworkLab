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


Use the Copper Straight-Through cable to connect PC0 and PC1 to Switch0(using FastEthernet0)  <br/>
<img src="https://i.imgur.com/Ijs6xXG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />


Connect Switch0 to PC0 and PC1(using FastEthernet0/1 and FastEthernet0/2)  <br/>
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

Connect Switch1 to PC2 and PC3(using FastEthernet0/1 to FastEthernet0/2)  <br/>
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




<h2>Configure the Router</h2>

- <b>Click on the router and navigate to the CLI tab
  </b>

- <b>You will be prompt with a message that reads "would you like to enter the initial configuration dialog?
- <b> Type no and click enter</br>
<img src="https://i.imgur.com/ffsIQx6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
  <b> Now in the user excution mode type "enable" and press enter
  <br />
<img src="https://i.imgur.com/pBoEnY6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
  <b> Now you are in the privleged mode. Type "configure terminal" and press enter.
  <br />
<br />
  <b> Now you are in the global configuration mode. This is where you configure the interface.(type interface g0/0 and click enter)
<img src="https://i.imgur.com/MtunX1f.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br />
<br />
  <b> Next you will assign an IP address.(type ip address 192.168.1.1 and the subnet mask 255.255.255.0) and press enter.
  

- <b> Next type no shutdown and press enter.
- <b> Now you can see interface g0/0 has changed to up.This means this port is now configured.

<img src="https://i.imgur.com/ORuW8my.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br />

<b> Now type exit to navigate back to you the global configuration mode. This is where you will configure the next interface.(type interface g0/1 and click enter)
- <b> Next you will assign another IP address.(type ip address 192.168.2.1 and the subnet mask 255.255.255.0) and press enter.
   <br />
- <b> Next type no shutdown and press enter.
- <b> Now you can see interface g0/1 has changed to up.This means this port is now configured.
 
<img src="https://i.imgur.com/CDU0IdK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


<h2>Configure the all PCs</h2>

- <b> Click on the PC0 and navigate to the desktop.
- <b> Click on IP Configuration
- <b> Type in IP address 192.168.1.10 subnet mask 255.255.255.0 
- <b> The default gateway will be your exiting router(192.168.1.1)
 <br />
  <img src="https://i.imgur.com/ygPnc7F.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
   
- <b> click on the PC1 and  navigate to the desktop.
- <b> click on IP Configuration 
- <b> Type in IP address 192.168.1.11 subnet mask 255.255.255.0
- <b> The default gateway will be your exiting router(192.168.1.1)
<br />
  <img src="https://i.imgur.com/SOqm5pw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    
- <b> Click on the PC2 and  navigate to the desktop.
- <b> Click on IP Configuration
- <b> Type in IP address 192.168.2.10 subnet mask 255.255.255.0
- <b> The default gateway will be your exiting router(192.168.2.1)
<br /> 
  <img src="https://i.imgur.com/hJ4BKiL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    
- <b> Click on the PC3 and  navigate to the desktop.
- <b> Click on IP Configuration
- <b> Type in IP address 192.168.2.11 subnet mask 255.255.255.0
- <b> The default gateway will be your exiting router(192.168.2.1)
<br />
  <img src="https://i.imgur.com/HkVF20A.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    
<h2>Connection is now established</h2>
<b> Now check the connection by sending a PDU from PC0 to the Router, PC02 - Router, PC0 - PC2.

<br />
  <img src="https://i.imgur.com/DVWKLPa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>



