---
layout: post
title: Cybersecurity
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

### DIGITALISATION

The digital economy has rapidly transformed the way businesses operate and interact with customers, and has brought about significant benefits such as increased efficiency, convenience, and innovation. However, this shift towards a more digital economy has also brought about new security implications, particularly in terms of cyber threats and vulnerabilities. In this response, I will examine the security implications of the digital economy based on the works of Wei et al. (2019) and Spremic and Simunic (2018), and provide my own reflections and thoughts on the subject.

Wei et al. (2019) define a 'fully digital enterprise' as an organization that has fully embraced digital technology in all aspects of its operations, from internal processes and communication to customer interactions and transactions. The authors note that while this digital transformation can bring about significant benefits, it also creates new vulnerabilities and potential security risks that must be addressed.

One of the major cyber security challenges associated with a fully digital enterprise is the increased risk of cyber attacks. As Spremic and Simunic (2018) note, the digitalization of business processes and data has made organizations more vulnerable to cyber threats such as hacking, malware, and ransomware attacks. In addition, the interconnectedness of digital systems means that a single breach can have far-reaching consequences, potentially affecting a large number of stakeholders.

Another challenge associated with a fully digital enterprise is the need to implement effective security measures across all aspects of the organization. This includes not just technical measures such as firewalls and encryption, but also policies and procedures to ensure that employees are aware of security risks and are trained to handle sensitive data securely. As Wei et al. (2019) note, a lack of security awareness and training can be a significant vulnerability in a fully digital enterprise.

In conclusion, the digital economy has brought about significant benefits and opportunities for businesses, but it has also created new security implications and challenges. A fully digital enterprise faces increased cyber security risks, and effective security measures must be implemented across all aspects of the organization. For bricks and mortar SMEs, becoming a digital enterprise can be particularly challenging, and additional resources and expertise may be needed to ensure that security risks are effectively managed. Finally, in light of the energy crisis, it is important to consider the sustainability of the digital economy and to balance the benefits of digital transformation with the need to reduce energy consumption and minimize environmental impact.

References:
Spremic, M., & Simunic, D. (2018). Cybersecurity challenges in the digital economy. Interdisciplinary Description of Complex Systems: INDECS, 16(3-B), 432-442.

### CYBERSECURITY THROUGH-OUT THE IoT LIFE CYCLE

<img width="903" alt="cybinIot" src="https://github.com/tayahlinus/tayahlinus.github.io/assets/154364754/eec43ee5-2b89-4d47-a2ac-65729fb737df">


Securing the Internet of Things (IoT) throughout its life cycle is crucial to mitigate the evolving threats and vulnerabilities associated with connected devices. The IoT life cycle typically involves the following stages: device manufacturing, device deployment, device operation, and device end-of-life. Here's how cybersecurity can be integrated into each phase:<br>

1. Device Manufacturing:<br>
   
a. Secure Boot and Firmware:
Implement secure boot mechanisms to ensure that only authenticated and authorized firmware is loaded onto the device.<br>

b. Device Identity Management:
Assign unique identifiers to each device to facilitate secure authentication and communication.<br>

c. Supply Chain Security:
Verify and secure the supply chain to prevent tampering or insertion of malicious components during the manufacturing process.<br>

d. Encryption and Secure Communication:
Implement strong encryption protocols for data in transit and ensure secure communication channels between devices and cloud services.<br>

2. Device Deployment:<br>
   
a. Authentication and Access Control:
Implement robust authentication mechanisms to ensure that only authorized users and devices can access the IoT ecosystem.<br>

b. Over-the-Air (OTA) Updates:
Enable secure and signed OTA updates to patch vulnerabilities and update device firmware throughout its operational life.<br>

c. Network Security:
Employ network segmentation and firewalls to isolate IoT devices from critical systems and limit the potential impact of a compromised device.<br>

d. Security Configuration:
Configure devices with the principle of least privilege, disabling unnecessary services and ensuring that default passwords are changed.<br>

3. Device Operation:
   
a. Continuous Monitoring:
Implement continuous monitoring of device behavior to detect anomalies or suspicious activities that may indicate a security breach.<br>

b. Data Encryption and Integrity:
Ensure end-to-end encryption of sensitive data and implement integrity checks to detect and prevent data tampering.<br>

c. Incident Response Plan:
Develop and implement an incident response plan to efficiently address and mitigate security incidents when they occur.<br>

d. User Education:
Educate end-users and administrators about security best practices, emphasizing the importance of strong passwords and security awareness.<br>

4. Device End-of-Life:<br>
   
a. Data Sanitization:
Ensure that all sensitive data is properly wiped or sanitized from the device before decommissioning to prevent data leakage.<br>

b. Secure Disposal:
Establish secure procedures for device disposal, including the physical destruction of components to prevent unauthorized access to residual data.<br>

c. Patch Management:
Provide a mechanism for secure end-of-life firmware updates to address any last-minute vulnerabilities.<br>

d. Regulatory Compliance:
Ensure compliance with data protection and privacy regulations during the decommissioning process.<br>

Conclusion:
Integrating cybersecurity throughout the entire IoT life cycle is essential for building a resilient and secure IoT ecosystem. This approach involves a combination of technical measures, user education, and adherence to best practices to address the evolving threat landscape and protect both the devices and the data they handle. Regular assessments, updates and a proactive security mindset are key elements in achieving a robust cybersecurity posture for IoT deployments.




