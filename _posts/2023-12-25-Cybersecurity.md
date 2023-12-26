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


