---
layout: post
title: IoT & Cybersecurity E-portfolio
subtitle:
categories: Website
tags: [Github, website]
---

## Cybersecurity <br>

### Scanning activity <br>

<strong>Results from performing a basic scan using traceroute:</strong><br>
1. Traceroute:
Use the 'traceroute' command to determine the number of hops from your machine to the assigned website. For example:<br>
traceroute yourwebsite.com<br>
Note the number of hops.<br>

2. Identify Delay:
Analyze the 'traceroute' output to identify the step causing the biggest delay. Note the average duration of that delay.<br>

3. Dig and Nslookup:
Use dig and nslookup to find information about the website's nameservers. For example:<br>
dig yourwebsite.com NS<br>
nslookup yourwebsite.com<br>
Note the main nameservers.<br>

4. Whois:
Use a 'whois' command to find information about the registered contact. For example:
whois yourwebsite.com<br>
Note the registered contact details.<br>

5. MX Record:
Use 'dig' to find the MX record for the website. For example:<br>
dig yourwebsite.com MX<br>
Note the MX record.<br>

6. Hosting Information:
Use online tools or commands like 'dig' to find where the website is hosted. For example:
dig yourwebsite.com A<br>
Note the IP address, and use online tools like IP lookup to find hosting information.<br>
Reflection:<br>
Issues or Challenges:
Challenges may arise due to firewalls, network restrictions, or incomplete DNS information.<br>
Overcoming Challenges:<br>
Try using alternative DNS servers.<br>
Use online tools or VPNs to overcome network restrictions.

### Solar Winds Article

[solarwinds1.docx](https://github.com/tayahlinus/tayahlinus.github.io/files/13772570/solarwinds1.docx)

### Honey Pot

We have successfully made and used a honeypot on ourselves here, now there are a couple of things i would like to touch on,
i believe this, in theory is great, however there are easier ways to do this that doesn't require you to use Kali at all, reducing the time and skill needed to make an actual honeypot, all you have to do is to go to any IP grabber website such as grabify, it could also redirect the user to a real website and the website URL can be changed to make it more believable, since if you are actually using this in real world people are less likely to click on 192.168.1.0:80 than to click on a link that says cutepuppies.com here's how it works, this is the home page:

<img width="923" alt="honeypot1" src="https://github.com/tayahlinus/tayahlinus.github.io/assets/154364754/80eefa4f-eada-44d6-bd37-fbc483142ffe">

We will just add any website we wish the target to be sent to after we grab their details, i'll use www.emu.edu.tr, then it asks you to customize the URL 

<img width="868" alt="honeypot2" src="https://github.com/tayahlinus/tayahlinus.github.io/assets/154364754/4cd20d41-99d4-4d9d-bef3-e221be24c226">

We can change the extention to make it even more realistic

<img width="915" alt="honeypot3" src="https://github.com/tayahlinus/tayahlinus.github.io/assets/154364754/d3d6df39-a053-4a3d-9b73-91a72bf30ad9">

As i said, any target is more likely to click on https://imghost.pics/join.php?id=EKLY83 compared to a random IP address, also setting it up is easy, takes less than a minute, here is how the website shows you the details of someone who clicked your link 

<img width="1118" alt="honeypot4" src="https://github.com/tayahlinus/tayahlinus.github.io/assets/154364754/1852de5d-69a6-4faa-8865-ca929087d2a4">

The exact same results, maybe even better, more realistic for the target since they will be redirected to an actual website and half the hassle for the person setting the trap, hope you enjoyed this experiment!

### DDOS
<strong>DDOS Attack</strong><br>
In this experiment we will be using Metasploit to flood a server with requests, making it unavailable for other users
to do this we need an IP address that we can obtain by using the scanning methods or honeypot that we talked about before
Let's say i didn't like the way apple made their new iphone so i'll be using their Website's IP address for the sake of this experiment, as of writing this the IP that i have obtained using Pingplotter for apple is : 17.253.144.10
we open Metasploit and we are met with this:

<img width="725" alt="DDOS1" src="https://github.com/tayahlinus/tayahlinus.github.io/assets/154364754/a7595afa-1164-45f8-80d2-c422787414fe">

Here we follow what the Doccument says: Then use the select the auxiliary “auxiliary/dos/TCP/synflood” by typing the following command. Msf6 > use auxiliary/dos/tcp/synflood Msf6> show options

<img width="1074" alt="DDOS2" src="https://github.com/tayahlinus/tayahlinus.github.io/assets/154364754/4058e440-f88a-4573-9587-bf10f30ffa5a">

And we follow buy inputting our IP address of choice, in this case apple's in the host section and then we type exploit, here's what we get:

<img width="1075" alt="DDOS3" src="https://github.com/tayahlinus/tayahlinus.github.io/assets/154364754/e471d10a-1b40-48e2-a5eb-93f51ceabf88">

We get an error here, after researching about the cause of this, it seems to be due to the way my OS has been configured, since i have installed KALI directly on mire drive (not using a VM) Kali does not recognize my wireless lan adapter and/or is not willing to use it, anyways, since the first time in class i have been trying to get this to work but it just doesn't seem to want to work, however we know the expected outcome from this and the cause,
the pro cybersecurity users always suggest to use a machine kali recommends, they also recommend desktops as suppoused to Laptops because there is better driver support for them, this error brings our experiment to an end here.

If this were to work, it would have not distrupted the apple's website since there is only one node spamming the website with requests, and my IP would probably get flagged for a couple of hours/days.






