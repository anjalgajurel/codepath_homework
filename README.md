# Honeypot Assignment

**Time spent:** **24** hours spent in total

**Objective:** Create a honeynet using MHN-Admin. Present your findings as if you were requested to give a brief report of the current state of Internet security. Assume that your audience is a current employer who is questioning why the company should allocate anymore resources to the IT security team.

### MHN-Admin Deployment (Required)

**Summary:** I used Google Cloud Platform to signup for cloud computing. There I registered for a free service to host up the virtual machine where I deployed the honeypots and the mhn-admin.

<img src="mhn-admin.gif">

### Dionaea Honeypot Deployment (Required)

**Summary:** Dionaea is a malware capturing honeypot. It traps malware exploiting vulnerabilities exposed by services offered over a network, and obtain a copy of the malware. It uses Python as its scripting language.

<img src="dionaea-honeypot.gif">

### Database Backup (Required) 

**Summary:** MHN-Admin uses MongoDB. The exported json file contains info about source port, destination port, timestamp, honeypot type, protocal, etc. Here is the link for the file. [session.json](/session.json)

### Deploying Additional Honeypot(s) (Optional)

#### Snort Honeypot

**Summary:** It is an open source network intrusion detection system that performs real-time traffic analysis. It can be used to detect a variety of attacks and probes, such as buffer overflows, stealth port scans, and OS fingerprinting attempts.

<img src="snort-honeypot.gif">

#### p0f Honeypot

**Summary:** p0f uses a fingerprinting technique based on analyzing the structure of a TCP/IP packet to determine  the  operating  system and other configuration properties of a remote host. The process is completely passive and does not generate any suspicious  network  traffic. This method can see thru packet firewalls and does not have the restrictions of an active fingerprinting.The main uses of passive OS fingerprinting are attacker profiling (IDS and honeypots), visitor profiling (content optimization), customer/user profiling(policy enforcement), pen-testing, etc.

<img src="p0f-honeypot.gif">

### Malware Capture and Identification (Optional)

#### WannaCry Malware

**Summary:** Dionaea captured this malware. It is a trojan virus which throws an error to user saying, "The application has failed to start ..." when the system starts.

MD5 Hash: *414a3594e4a822cfb97a4326e185f620*

SHA1 Hash: *5f1e7bc375dd8093fa987af0771e72389dad473b*

<img src="wannacry-malware.png">

#### Kido Worm

**Summary:** Dionaea found the malware. It is also called Conficker. This worm mainly spreads through local network and external storage devices such as USB, portable hard drives, etc. It will back up the executable files to the system with random names.

MD5 Hash: *af76a2ad1dc8525e73a5c6dc932c7913*

SHA1 Hash: *c680a4e34b71a4f27b6b50b7f1641d1769ff048f*

<img src="kido-malware.png">

## Notes

It took me a while to figure out what all this assignment is about. After going through the steps, it was a breeze setting up the honeypots. I had issues while deploying Suricata and Glastopf. Also, I was having authentication issues with one of the VMs. 
