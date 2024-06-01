# Home Lab

## Objective

This project aims to provide a safe and controlled environment in which I can analyze malware, while also providing basic telemetry that can be investigated with Splunk.

### Skills Learned

- Basic understanding of SIEM concepts and practical application.
- Ability to generate and investigate data.
- Virtual Machines configuration
- Basic payload creation
- Creation of a separate environment from my network, in order to analyze malware.
- Development of critical thinking and problem-solving skills in cybersecurity.

### Tools Used

- Security Information and Event Management (SIEM) system for log ingestion and analysis - Splunk
- Telemetry generation tools to create realistic network traffic and attack scenarios - Nmap, Metasploit Venom

## Steps


## STEP 1 - Setting up the VMs (Windows 10 & KaliLinux)
![image](https://github.com/carageadenis1806/Home-Lab/assets/75758209/3c62d748-cab2-4f8e-a121-a167560a304a)



## STEP 2 - Configuring the VMs into a LAN segment

![image](https://github.com/carageadenis1806/Home-Lab/assets/75758209/ee6289dc-b27c-4607-a034-a8a89f98be3c)

*Ref 1: VMs network config from Vmware.*

*Ref 2: Windows machine network config.*

*Ref 3: Kali machine network config.*

*Ref 4: Checking the connectivity between the machines.*



## STEP 3 - Installing Splunk & Sysmon



## STEP 4 - Crafting the payload using MSFvenom

![image](https://github.com/carageadenis1806/Home-Lab/assets/75758209/d2f62b35-1769-44a3-9f6b-63b57d147488)

*Ref 1: Creating a reverse TCP payload named Chestionar.pdf.exe*

*Ref 2 & 3: Configuring the payload.*

*Ref 4: Starting a web server from which we can download the payload on the Windows machine.*



## STEP 5 - Delivering the payload

![image](https://github.com/carageadenis1806/Home-Lab/assets/75758209/4217474e-a1ff-4c10-9475-b9b7d8d69061)

*Ref 1: Accesing the Kali web server from the windows machine and downloading the payload.*

## STEP 6 - Obtaining Command and Control
![image](https://github.com/carageadenis1806/Home-Lab/assets/75758209/b98faba1-c8f4-423c-a71b-132ded93e41a)

*Ref 1: Once the payload has been executed on the Windows machine, we have remote access to it from the Kali machine.*

*Ref 2: We open a shell so that we can execute basic commands that provide basic telemmetry for Splunk to ingest.*

## STEP 7 - Investigating ingested data with Splunk

![image](https://github.com/carageadenis1806/Home-Lab/assets/75758209/ae6d1bb1-9ee8-421c-8299-ee2bac2c7446)


