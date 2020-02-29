# Kali Build

Kali is the de-facto Linux penetration testing distribution. It makes it very easy to get up and running so you're not wasting tons of time on prep.

## Install Kali

[Get Kali](https://www.kali.org/downloads/) - I typically use the 64-bit version. The installer is for if you want to install it to media (recommended), but the Live CD is also useful.

Use disk encryption with a strong password, especially if this is for any sort of real testing. 

## Update Kali

Kali is a rolling distribution, so updates are available all the time. The version of Kali from the website is just a snapshot in time, so you'll probably want to update Kali before you go further. Depending on how old the image you downloaded is, there may be hundreds or thousands of packages to update.

That said, you don't actually always need the latest and greatest for things like CTFs and conferences.

To update: `apt update && apt upgrade -y`

## Install Extra Tools

This is a matter of personal taste, but there are packages and 3rd party tools that can be beneficial. This list has grown over time with friends adding to it, so some packages may be already installed. However, by including them here, it ensures they're up-to-date, even if you didn't update the entire system.

### Packages

`apt update && apt install -y aircrack-ng automake autotools-dev beef-xss bless bloodhound brasero bridge-utils dhcpdump ettercap-graphical exfat-fuse file-roller filezilla filezilla-common freetds-bin freetds-common freetds-dev freerdp-x11 gdebi gedit gobuster gparted gvfs-fuse htop ipv6toolkit isc-dhcp-server libical-dev libncurses5 libpam-winbind libpam0g libreoffice linux-libc-dev mimikatz nethogs netsed p7zip p7zip-rar powersploit pure-ftpd rar responder rinetd screen seclists sqsh ssdeep sshfs sshpass swig3.0 terminator tftpd thc-ipv6 tmux unace unrar unzip usbip veil veil-catapult veil-evasion webshells wmis zip`

Some noteable items:
- Bloodhound - Great tool for identifying how to move laterally and gain administrator access in Active Directory networks.
- exfat - Filesystem that is nice to install because Windows, OS X, and Kali can all read/write it and there's no technical limits (like small max filesize with FAT) that will slow you down.
- mimikatz - Popular credential extractor for Windows targets.
- SecLists - Good lists for scanners and password guessing
- Veil - PSP evasion toolkit

### Browser Plugins

- NoScript
- Quick-Proxy
- Cookies Manager+
- Live HTTP Headers (Clone)
- Tamper Data

### Other Free Goodies

- [CyberChef](https://github.com/gchq/CyberChef) - Analysis toolkit that lets you rapidly prototype
- [Ghidra](https://ghidra-sre.org/) - Free, robust RE toolkit with way more support than IDA Free
- Powershell Empire - Powershell-based C2 framework
  - Install: `git clone https://github.com/EmpireProject/Empire.git`
  - Setup: `setup/install.sh`
  - Check: Make sure it has modules it in once you run it, otherwise something went wrong
- [Visual Studio Code](https://code.visualstudio.com) - GUI text editor
- [Sysinternals Suite](https://docs.microsoft.com/en-us/sysinternals/downloads/sysinternals-suite) - Lots of great Microsoft tools for Windows targets

### Other Paid Goodies

- BurpSuite Pro - There's a free version on Kali already, but the Pro version is relatively affordable and useful
- Cobalt Strike - Popular Red Team C2 framework
- Nessus Pro
- CORE Impact - Real nice, real expensive

## Tweak

- Veil - Even though you installed it from apt, you still need to run veil for some first-time installation stuff. Takes 30+ minutes.
-	Bloodhound -  Even though you installed it from apt, you need to follow some [extra instructions](https://stealingthe.network/quick-guide-to-installing-bloodhound-in-kali-rolling/) to set up the graph DB. 
- Run `ssh-keygen -t rsa -b 4096` to generate SSH keys for root. These are nice before cloning so everyone on the team has the same keys, making it easy to share backdoor'd SSH accounts. Recommended to put a password on this key, because you're probably going to be using it for admin access within your target network.

## Bag of Toys

You may want to consider bringing some of the following, depending on what you're doing:

- Duffle bag
- CD-R/CD-RW/DVD-R/DVD-RW
- CD/DVD external drive writer
- USB flash drives
- USB Ethernet adapters (Kali-compatible)
- USB powered hub
- USB mice
- USB keyboards
- USB wireless adapters (Kali-compatible)
- Ethernet cables
- Unmanaged Ethernet switch(es)
- Power strips
- Power extension cords
