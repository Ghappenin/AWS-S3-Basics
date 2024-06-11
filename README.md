# AWS-S3-Basics

<h2>Description</h2>
By the end of this lab, you will create S3 bucket and will be able upload content to the bucket. You will also enable Encryption, Versioning for S3 Bucket and will create Lifecycle management rule for objects in S3 Bucket.  You will also create a Static website using AWS S3.



<br />


<h2>Operating System Used<h2>

- <b>WIndows 11 Home 13th Gen Intel(R) Core(TM) i7-1360P 2.20 GHz</b>

<h2>Downloads<h2>
 
- <b>[AWS](https://aws.amazon.com/free/?gclid=CjwKCAjwyJqzBhBaEiwAWDRJVLXvkQI5wJoWiiJhWEcL25WlnjIhO4V67lEnaaDeBi1qYFqEwQBZbBoCQFUQAvD_BwE&trk=fce796e8-4ceb-48e0-9767-89f7873fac3d&sc_channel=ps&ef_id=CjwKCAjwyJqzBhBaEiwAWDRJVLXvkQI5wJoWiiJhWEcL25WlnjIhO4V67lEnaaDeBi1qYFqEwQBZbBoCQFUQAvD_BwE:G:s&s_kwcid=AL!4422!3!432339156150!e!!g!!aws!1644045032!68366401852&all-free-tier.sort-by=item.additionalFields.SortRank&all-free-tier.sort-order=asc&awsf.Free%20Tier%20Types=*all&awsf.Free%20Tier%20Categories=*all)</b>

<h2>Project walk-through:</h2>

<p align="center">
Create an AWS account: <br/>
<img src="https://i.imgur.com/xvH50D5.png" height="80%" width="80%" />
<br />
<br />
Select the region of your liking: <br/>
<img src="https://i.imgur.com/514Gq2W.pngg" height="80%" width="80%" />
<br />
<br />
Upper left of screen next to Services search "S3" and click on "Scalable Storage in the Cloud: <br/>
<img src="https://i.imgur.com/SQrYHxE.png" height="80%" width="80%" />
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
