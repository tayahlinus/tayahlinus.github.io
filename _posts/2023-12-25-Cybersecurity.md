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

