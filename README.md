# Repository of Security Resources

A starting point for you to begin, or grow, your cybersecurity knowledge. This has a US-focus, with some specific details for the Baltimore/DC area.

There is enough on this page to keep you busy for months. The key to successful people in cybersecurity is putting in effort. If you're lucky, you can do that through your job. Otherwise, find ways to put in the time, like podcasts during your commute, conferences with friends, etc. I do not believe you need to spend all of your time outside of your job to be great, but if you enjoy spending *some* time outside of work tinkering, it will certainly benefit you.

## Podcasts

I strongly recommend listening to podcasts on your commute and/or whenever else you have free time (like when working out)! It is a great way to learn and stay in touch with the industry/community. I use Podcast Addict for Android, but there are many apps that support podcasts.

Listed in order of preference, but if I find it worth listening to if I listed it (unless otherwise noted).

### Cybersecurity

- *Risky Business*
- *Defensive Security* - Great podcast, but less frequent right now due to health issues of the host.
- *SANS Internet Storm Center Daily*
- *Brakeing Down Security*
- *The Cyberlaw Podcast* by Steptoe
- *Darknet Diaries* - Only stories, but you can learn something from a good story!
- *Security Weekly* (and other shows on the network) - Good discussions, but frequently overly raunchy and off-topic.


In my opinion, you should avoid *Security Now*. While it is more accessible to newcomers, the hosts are frequently wrong and it is hard to know that they're wrong unless you have more experience.

### National Security

National security frequently involves cybersecurity and privacy issues that affect our daily lives. These podcasts frequently touch on these issues, along with other issues you may find interesting given your security background.

Listed in order of preference, but I find them all good:

- *Bombshell*
- *The National Security Law Podcast*
- *The Lawfare Podcast*
- *Rational Security*
- *War on the Rocks*

## Whitepapers

*Resilient Military Systems and the Advanced Cyber Threat* by Defense Science Board - Report on cyber vulnerabilities in US military systems, referenced frequently for it's threat tier system. It's from 2013, but still relevant. [OSD DSB](https://dsb.cto.mil/reports/2010s/ResilientMilitarySystemsCyberThreat.pdf)

*APT1* by FireEye/Mandiant - Original report calling out a specific Chinese military organization as a persistent threat actor. [FireEye](https://www.fireeye.com/content/dam/fireeye-www/services/pdfs/mandiant-apt1-report.pdf)

*DBIR* by Verizon - Annual report on the state of how criminals/APTs are getting in and what their goals are. [Verizon](http://www.verizonenterprise.com/verizon-insights-lab/dbir/)

## Websites

*OWASP Top Ten* by OWASP - The most common and critical web application vulnerabilities. [OWASP](https://www.owasp.org/index.php/Category:OWASP_Top_Ten_Project)

*ATT&CK* by MITRE - A common language for identifying how attackers operate, particularly useful for defenders trying to understand what gaps they have. [MITRE](https://attack.mitre.org/)

## Books

*Countdown to Zero Day: Stuxnet and the Launch of the World's First Digital Weapon (2015)*	by Kim Zetter - Great context and story about Stuxnet and other malware. Extremely eye-opening and is the perfect real-world example to contradict people saying "no one could do that." [Amazon](https://www.amazon.com/Countdown-Zero-Day-Stuxnet-Digital/dp/0770436196) or your local library

*The Cuckoo's Egg* by Chris Stoll - Story of an intrusion into US Air Force networks decades ago, yet most of the problems are still relevant. [Amazon](https://www.amazon.com/Cuckoos-Egg-Tracking-Computer-Espionage/dp/1416507787) or your local library

Palo Alto Cybersecurity Cannon - Curated list of great cybersecurity books, updated yearly. [Palo Alto](https://cybercanon.paloaltonetworks.com/)

## Conferences

There are many popular conferences that may be worth attending. Each one has a different feel - some are more business oriented (i.e., vendors selling products) and others are more hacker oriented (i.e., focus is on the tech and hacking/defending things). Both are good and necessary, just different vibes.

- [BSides](http://www.securitybsides.com/w/page/12194156/FrontPage) are local conferences, frequently associated with a major city/town. Typically very affordable. There are many BSides of different sizes, so search for your own city, or start your own event.
  - [BSidesDC](http://www.bsidesdc.org/) - Washington DC event, typically October/Fall.
  - [BSidesCharm](http://www.bsidescharm.com/) - Baltimore event, typically April/Spring.
  - [BSides Las Vegas](https://www.bsideslv.org/) - Las Vegas event, typically August in the middle of Black Hat and DEF CON.
  - [BSides NoVA](http://www.bsidesnova.org/) - Northern Virginia event, typically March.
- [DEF CON](https://defcon.org/) - Las Vegas, typically early August, very large, hacker oriented with lots of villages and hands-on activities.
- [Black Hat](https://www.blackhat.com/) - Las Vegas, typically early August, very business oriented.
- [USENIX Security](https://www.usenix.org/conference/usenixsecurity19) - Location changes, August, research focus.
- [RSA](https://www.rsaconference.com/) - San Fransico, typically February/March, very big conference, very business oriented.
- [Schmoocon](https://shmoocon.org/) - Washington DC, very popular conference, hard to get tickets.
- [Derbycon](https://www.derbycon.com/) - Very popular conference, held it's tenth and final event in September 2019.

"Hacker Summer Camp" is a term that refers to typically the last week of July or first week of August. Black Hat, BSides Las Vegas, and DEF CON all occur that same week in Las Vegas, overlapping somewhat.

Nearly all these conferences post video recordings of the talks on YouTube. You can look through old conference schedules to see what seems interesting and then search YouTube for the talk title.

## Capture the Flag (CTF) Events
- [Holiday Hack Challenge](https://holidayhackchallenge.com/past-challenges/) - SANS runs a CTF every December for prizes, but the previous challenges are still running and fun.
- Many conferences and universities have CTFs, some require you to be there, others are remote. 

## Practice Virtual Machines (VMs)

***If you download an intentionally vulnerable virtual machine (VM), it is your responsibility to make sure that this VM is not accessible to the Internet. It's best to not even expose this VM to an internal home network. The safest way is to use an host internal network, so the vulnerable VM can only be accessed by other VMs on the system.***

- [OverTheWire](https://overthewire.org/wargames/) - Fun mini challenges, highly recommend tinkering here.
- [Hack the Back](https://www.hackthebox.eu/) - Lab environment with many vulnerable machines. Free, but if you pay you have a better experience. Great practice range where you spend your time learning, not fussing with VMs and infrastructure.
- [Metasploitable 3](https://github.com/rapid7/metasploitable3) and [Metasploitable 2](https://sourceforge.net/projects/metasploitable/) - Vulnerable VMs from Rapid7. Metasploitable 3 is nice because it's a Windows target, but is more work to build.
- [VulnHub](https://www.vulnhub.com/) - Lots of VMs, see [here](http://www.abatchy.com/2017/02/oscp-like-vulnhub-vms) and [here](https://medium.com/@a.hilton83/oscp-training-vms-hosted-on-vulnhub-com-22fa061bf6a1) for a sublist of interesting ones.

## Tools

- [Kali](https://kali.org) - Linux distribution commonly used for penetration testing and CTFs
- [CyberChef](https://gchq.github.io/CyberChef/) - Toolset for extracting and operating on data, great for CTFs and work too.

## Movies

- War Games
- Sneakers
- Hackers
