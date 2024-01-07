# Enumerator <br>
### ${\textcolor{blue}{A \ Customized \ Virtual \ Machine \ for \ OSINT \ on \ Website}}$
The Enumerator is a custom-created virtual machine (VM) managed on Kali Linux, tailored for Open-Source Intelligence (OSINT) operations on a targeted website. It features a curated set of tools pre-installed on Kali Linux, including specialized Firefox extensions and other online tools, to facilitate efficient information gathering. Additionally, the VM is equipped with extra tools that have been installed to augment its capabilities. This comprehensive approach, combining both local and additional tools, enhances the Enumerator's effectiveness in conducting thorough website reconnaissance during OSINT activities.

## Tools <br>
### Blackbird <br>
**Description:** <br>
Blackbird is a tool designed for information gathering and reconnaissance. It collects data related to a target website, focusing on extracting information about its subdomains, IP addresses, and possible vulnerabilities. <br>

**Information Gathered:** <br>
* Search for accounts by username across 153 sites. <br>
* Find active profiles on various social media sites. <br>

**Usage Example:**
`python blackbird.py -u <target username>`

**Guide Link:** [Blackbird](https://github.com/p1ngul1n0/blackbird) <br>

### Metagoofil <br>
**Description:** <br>
Metagoofil is a metadata gathering tool that extracts valuable information from publicly available documents, such as PDFs, Word documents, and presentations. It helps in revealing sensitive information that might be inadvertently disclosed in the document metadata. <br>

**Information Gathered:** <br>
* Metadata from documents, including author names, software used, and timestamps. <br>
* Document-related information, such as file names and paths. <br>

**Usage Example:**
`metagoofil -d <target domain> -t doc,pdf -l 200 -n 50 -o <path where results to be stored> -f <file name with .html where results to be stored>`

**Guide Link:** [Metagoofil](https://www.kali.org/tools/metagoofil/) <br>

### WHOIS Lookup <br>
**Description:** <br>
WHOIS Lookup is a tool used to query domain registration databases to obtain information about the ownership, registration date, and contact details of a domain name. <br>

**Information Gathered:** <br>
* Domain ownership details (registrant name, organization, etc.). <br>
* Registration and expiration dates. <br>
* Name server information. <br>
* Contact details of the domain owner. <br>

**Usage Example:**
`whois <target domain>`, `whois <target IP>`

**Guide Link:** [WHOIS Lookup](https://www.geeksforgeeks.org/how-to-use-the-whois-command-on-ubuntu-linux) <br>

## Extensions <br>
### Wappalyzer - Technology Profiler <br>
**Description:** <br>
Wappalyzer is a technology profiler that identifies the technologies used by a website. It detects content management systems, web frameworks, server software, and more, providing insights into the technology stack employed by the target site. <br>

**Information Gathered:** <br>
* Content Management System (CMS) being used. <br>
* Web frameworks and libraries utilized. <br>
* Server software and hosting details. <br>

**How to Add:** <br>
Wappalyzer can be added to Firefox as an extension. You can find it on the official Firefox Add-ons website. Simply click on "Add to Firefox" to install the extension. <br>

### Shodan <br>
**Description:** <br>
Shodan is a search engine for internet-connected devices. It allows users to discover and explore devices connected to the internet, including servers, routers, webcams, and more. Shodan provides information about open ports, services running on those ports, and sometimes even specific vulnerabilities. It's widely used for both security research and reconnaissance. <br>

**Information Gathered:** <br>
* Open ports and services on a target server. <br>
* Details about connected devices, including type and manufacturer. <br>
* Vulnerabilities and misconfigurations. <br>

**How to Add:** <br> 
Shodan provides a Firefox extension that can be added from the Mozilla Add-ons website. Click on "Add to Firefox" to install the Shodan extension. <br>

### Link Gopher <br>
**Description:** <br>
Link Gopher is a Firefox extension that extracts and lists all the links (URLs) on a webpage. It simplifies the process of collecting and analyzing the links present on a website. <br>

**Information Gathered:** <br>
* List of all links on a webpage. <br>
* URL details, including target destinations. <br>

**How to Add:** <br>
Link Gopher can be added to Firefox through the Mozilla Add-ons website. Click on "Add to Firefox" to install the Link Gopher extension. <br> 

## Kali Linux Built-in Tools <br>
### The Harvester <br>
**Description:** <br>
The Harvester is a reconnaissance tool used for gathering information about email addresses, subdomains, and other related information regarding a target. It collects data from various public sources, including search engines, PGP key servers, and Shodan. The Harvester is particularly useful for information gathering during the initial phases of penetration testing or ethical hacking. <br>

**Information Gathered:** <br>
* Email addresses associated with the target domain. <br>
* Subdomains of the target domain. <br>
* Hostnames associated with the target. <br>

**Usage Example:**
`theHarvester -d <target domain> -l 300 -b all`

**How to Access:** <br>
The Harvester is pre-installed in Kali Linux. You can access it from the terminal by typing: theharvester. <br>

### Nmap (Network Mapper) <br>
**Description:** <br>
Nmap is a powerful open-source tool for network exploration and security auditing. It is used to discover hosts and services on a computer network, creating a map of the network's structure. Nmap employs various scanning techniques to gather information about open ports, running services, and the operating systems of target machines. It is widely used by security professionals for network reconnaissance and vulnerability assessment. <br>

**Information Gathered:** <br>
* Open ports on target systems. <br>
* Services running on those ports. <br>
* Version information about the services. <br>
* Operating system detection. <br>

**Usage Example:**
`nmap <target domain>`, `nmap <target IP>`

**How to Access:** <br>
Nmap is also pre-installed in Kali Linux. You can access it from the terminal using the nmap command, followed by the target IP or hostname. For example: nmap target.com. <br>

## Online Available Tool <br>
### Skymem <br>
**Description:** <br>
Skymem is the website which helps you find the email address of any professional, person or company. We collect and organize email addresses from all over the web. <br>

**How to Search on Skymem:** <br>
1. Start with a simple search using a domain name: eg. wdc.com or ferguson.com. <br>
2. Type a full email address, eg.: daniel.warner@ferguson.com <br>
3. Type first and last name separated with '.' or '_' or '-' and find that person or similar under other domain/company, like this: david.baker <br>
4. Type first and last name with a domain name and we will do our best to find the email of that person. <br>
eg. david baker exeloncorp.com <br>

**Guide Link:** [Skymem](https://www.skymem.info/) <br>

# Disclaimer <br>
These tools are intended for educational purposes and legal use only. The authors and contributors are not responsible for any misuse, damage, or legal consequences caused by the use of this tool. Please use responsibly. 
