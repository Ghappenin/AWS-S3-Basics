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
Upper left of screen next to Services search "S3" and click on "Scalable Storage in the Cloud": <br/>
<img src="https://i.imgur.com/SQrYHxE.png" height="80%" width="80%" />
<br />
<br />
Click "Create Bucket" -> give bucket a "name" -> keep Object Ownership to "ACLs disabled":  <br/>
<img src="https://i.imgur.com/fyNgiJn.png" height="80%" width="80%" />
<br />
<br />
Block all public access:  <br/>
<img src="https://i.imgur.com/Zc1RHDZ.png" height=80%" width="80%" />
<br />
<br />
Bucket Versioning "disabled" -> Give Tags Key "name" and Value "name" -> keep default encryption -> click "create bucket":  <br/>
<img src="https://i.imgur.com/rFVeO28.png" height="80%" width="80%" />
<br />
<br />
You have successfully created an AWS S3 Bucket <br/>
<img src="https://i.imgur.com/wyrx2uS.png" height="80%" width="80%" />
<br />
  - <b>https://aws.amazon.com/s3/
<br />
<br />
Now Upload Object to S3 and Manage Access using bucket Policies and ACLs -> First, click into your bucket: <br/>
<img src="https://i.imgur.com/WEQmNNr.png" height="80%" width="80%" />
<br />
<br />
Click "Create Folder" -> Give the folder a "name", keep encryption defualt -> click "Create Folder" <br/>
<img src="https://i.imgur.com/T5uKRgR.png" height="80%" width="80%" />
<br />
<br />
Click into your folder -> click "upload": <br/>
<img src="https://i.imgur.com/3HHpINa.png" height="80%" width="80%" />
<br />
<br />
Click "add files" <br/>
<img src="https://i.imgur.com/1TP8MXj.png" height="80%" width="80%" />
<br />
<br />
Add File: <br/>
<img src="https://i.imgur.com/HbYfod4.png" height="80%" width="80%" />
<br />
<br />
Notice Destination settings are that of what we selected previously: <br/>
<img src="https://i.imgur.com/vnhpdJx.png" height="80%" width="80%" />
<br />
<br />
Scroll to "Properties" -> Keep storage "Standard": <br/>
<img src="https://i.imgur.com/4gd39xS.png" height="80%" width="80%" />
<br />
<br />
Under "Permissions" find your Access Control List (ACL) -> keep permissions to yourself "Object Owner" -> Click "Upload": <br/>
<img src="https://i.imgur.com/6TrKd3f.png" height="80%" width="80%" />
<br />
<br />
To verify download was successful click into the file -> upper right click "open" your image/file should open<br/>
<img src="https://i.imgur.com/G4s2UEB.png" height="80%" width="80%" />
<br />
<br />
If you attempt to open with "Object URL" you will get this screen -> When bucket was created we did so with "NO" public access <br/>
<img src="https://i.imgur.com/iCVddRW.png" height="80%" width="80%" />
<br />
<br />
To change this go back to "bucket" -> click "Permissions" -> Unclick "block all public access" -> Save changes -> "Confirm" <br/>
<img src="https://i.imgur.com/Ugpct9z.png" height="80%" width="80%" />
<br />
<br />
To change encryption move over to the "properties" tab -> choose between "SSE-S3", "SSE-KMS" or "DSSE-KMS" <br/>
<img src="https://i.imgur.com/9u23d0r.png" height="80%" width="80%" />
<br />
   -As of January 5th, 2023 all object uploads to S3 are automatically encrypted at no extra cost.
   
<br />
Visit a web page and detect its IP address using a display filter. A TLS handshake display filter: tls.handshake.type ==1 <br/>
<img src="https://i.imgur.com/LoPi1bu.png" height="80%" width="80%" />
<br />
<br />

