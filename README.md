# AWS-S3-Basics

<h2>Description</h2>
Project consists of downloading current operating system version of Wireshark. By the end of this lab, you will create S3 bucket and will be able upload content to the bucket. You will also enable Encryption, Versioning for S3 Bucket and will create Lifecycle management rule for objects in S3 Bucket.  You will also create a Static website using AWS S3.



<br />


<h2>Operating System Used<h2>

- <b>MacOS Monterey Version 12.7.4</b>

<h2>Downloads<h2>
 
- <b>[Wireshark 4.2.4 Intel](https://www.wireshark.org/)</b>

<h2>Project walk-through:</h2>

<p align="center">
Download Wireshark: <br/>
<img src="https://i.imgur.com/FVWrYiX.png" height="80%" width="80%" />
<br />
<br />
Select source of capture: Wireless, Ethernet etc: <br/>
<img src="https://i.imgur.com/00SfRUR.png" height="80%" width="80%" />
<br />
<br />
Upper left click -green- "sharkfin" to begin your capture: <br/>
<img src="https://i.imgur.com/lbyR5hY.png" height="80%" width="80%" />
<br />
<br />
Stop your capture with -red- box and save to your file of choosing:  <br/>
<img src="https://i.imgur.com/UN55BQU.png" height="80%" width="80%" />
<br />
<br />
Use a display filter to detect HTTPS packets:  <br/>
 ●To display certain packets in an existing packet capture, use a display filter <br/>
 ●To display only HTTPS traffic, use a filter on TCP port 443: tcp.port == 443 <br/>
<img src="https://i.imgur.com/W2nbWQN.png" height=80%" width="80%" />
<br />
<br />
Use a display filter to detect DNS (Domain Name System)if websites and subsites visited:  <br/>
<img src="https://i.imgur.com/2xEq9cr.png" height="80%" width="80%" />
<br />
 - <b>https://wiki.wireshark.org/DisplayFilters
<br />
<br />
Visit a web page and detect its IP address using a display filter. A TLS handshake display filter: tls.handshake.type ==1 <br/>
<img src="https://i.imgur.com/LoPi1bu.png" height="80%" width="80%" />
<br />
<br />
●A Conditional statement may be used to include and eliminate packets from a Wireshark capture: !(ip.addr == 8.43.85.97) and tcp.port == 443

●A compound conditional should include parentheses to avoid order of execution errors: !(ip.addr == 8.43.85.97) and (tcp.port == 80 or tcp.port == 443)
