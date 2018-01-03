# VM Detection

Compilation of things to look for when identifying if you're on a VM or physical system.

Detection
Try to connect out to cnn.com
/proc/cpuinfo
egrep "uml" /proc/ksysms 
egrep "honey" /proc/ksysms 
/etc/group
/etc/passwd
User action history
Printers are all generic or there are none
Network uses TUN/TAP
Existance of UML
lspci for hypervisor
MACs of VM infrastructure
	Company and Products								MAC unique identifier (s)
	VMware ESX 3, Server, Workstation, Player			00-50-56, 00-0C-29, 00-05-69
	Microsoft Hyper-V, Virtual Server, Virtual PC		0-03-FF
	Parallells Desktop, Workstation, Server, Virtuozzo	00-1C-42
	Virtual Iron 4										00-0F-4B
	Red Hat Xen											00-16-3E
	Oracle VM											00-16-3E
	XenSource											00-16-3E
	Novell Xen											00-16-3E
	Sun xVM VirtualBox									08-00-27
CPUID https://kb.vmware.com/selfservice/microsites/search.do?language=en_US&cmd=displayKC&externalId=1009458
dmidecode 
	http://old.honeynet.org/papers/individual/DefeatingHPs-IAW05.pdf
chroot detection with ls -ialgG, inodes on root should be '2'
jail detection with ps, looking for the "J" flag


The machine looks like it was just set up yesterday and the only thing it has on it besides default directories is a folder called "Sensitive" filled with page scans of old copies of 2600 and lists of mispelled names and address purporting to be employees of HB Gary.
The mouse driver has the manufacturer labeled as "Microsoft SMS Solutions"
You try to talk to the drive controller or any other DMA device and the computer begins responding like it had a lobotomy.
The CPUID op code places value 0x02 in EAX
You do an RDTSC timing on an instruction sequence and the resulting value is some insane number.
You try to make an HTTP connection to cnn.com and get the error "cannot connect"
The only printers installed on the machine have the word "generic" in their name.
You give the command "net view" and get back the response "The list of servers for this workgroup is not currently available."
Your radio scanner suddenly has a lot of wierd activity on Motorola trunking lines by guys with Texan accents saying things like "Code 10" and "in position".
